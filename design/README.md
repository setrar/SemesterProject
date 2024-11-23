

## Division of roles (between the OAI PHY layer and the RF board)

When using **BladeRF** with **OpenAirInterface (OAI)**, the division of roles between the OAI PHY layer and the RF board (and specifically the FPGA on the RF board) is as follows:

---

### **OAI PHY Layer Role**
The OAI PHY layer processes the baseband signal, which includes modulation, channel coding, and any other baseband signal processing functions necessary for the LTE or 5G signal. 

1. **Transmit Path:**
   - The PHY layer generates **IQ samples** for transmission after tasks such as:
     - **Channel Coding**: Turbo codes (LTE) or LDPC (5G NR).
     - **Modulation**: QPSK, 16QAM, or 64QAM symbols.
     - **OFDM Modulation**: Adding cyclic prefixes and generating time-domain samples through the IFFT.
     - **Beamforming (if applicable)**: Applying weights to IQ streams for directional transmission.

2. **Receive Path:**
   - The PHY layer processes the received **IQ samples** after the RF board has converted the analog signal to digital:
     - **OFDM Demodulation**: Removing the cyclic prefix and performing FFT to retrieve frequency-domain data.
     - **Channel Estimation and Equalization**: Correcting for channel effects using pilot symbols (e.g., DMRS).
     - **Demodulation**: Extracting bits from QPSK/16QAM/64QAM symbols.
     - **Channel Decoding**: Turbo or LDPC decoding to retrieve the final bit stream.

---

### **RF Board Role (BladeRF FPGA and RF Frontend)**
The RF board's **FPGA** handles the tasks that interface between the digital baseband signal and the RF domain. These tasks typically include:

1. **Transmit Path:**
   - **Digital Upsampling and Filtering**: The IQ samples from the OAI PHY layer are interpolated and filtered for transmission.
   - **Digital-to-Analog Conversion (DAC)**: Converts the digital IQ samples to an analog signal.
   - **RF Upconversion**: Mixes the analog baseband signal to the desired RF frequency for over-the-air transmission.

2. **Receive Path:**
   - **RF Downconversion**: Converts the received RF signal from the carrier frequency to baseband.
   - **Analog-to-Digital Conversion (ADC)**: Converts the analog baseband signal to digital IQ samples.
   - **Digital Downsampling and Filtering**: Decimates and filters the digital samples before sending them to the OAI PHY layer.

3. **Clock Synchronization**: Ensures tight timing control for sample rates and carrier frequencies, often with GPS or external clocks for synchronization in testbeds.

4. **FPGA-Specific Tasks**:
   - **IQ Balancing and Correction**: Corrects imperfections in the RF hardware, such as IQ imbalance and DC offset.
   - **Timing Control**: Handles precise sample timing to align with OAI's real-time processing requirements.
   - **Optional Beamforming**: May implement basic beamforming tasks if the FPGA supports it.

---

### **Understanding the FPGA's Role**
The FPGA acts as a **bridge between the digital domain (OAI) and the analog/RF domain**. Its tasks ensure the digital IQ samples are ready for RF transmission and that incoming RF signals are correctly converted back to IQ samples for baseband processing. 

---

### **Summary of Signal Flow**
1. **Transmit Path**: OAI PHY → IQ Samples → BladeRF FPGA (Upsampling, DAC, Upconversion) → RF Signal.
2. **Receive Path**: RF Signal → BladeRF FPGA (Downconversion, ADC, Downsampling) → IQ Samples → OAI PHY.

The **FPGA** in the BladeRF board performs critical real-time signal processing tasks that cannot be efficiently managed by a general-purpose CPU or software stack like OAI, given the high sampling rates and tight timing requirements in modern wireless systems.
