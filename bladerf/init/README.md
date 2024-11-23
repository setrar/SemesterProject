# Init Board

To download the FPGA bitstream file for the bladeRF 2.0 micro xA4 using curl, execute the following command in your terminal:

```
curl -O https://www.nuand.com/fpga/hostedxA4-latest.rbf
```
> Returns
```powershell

  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
100 2570k    0 2570k    0     0   555k      0 --:--:--  0:00:04 --:--:--  607k
```

This command retrieves the file hostedxA4-latest.rbf from the specified URL and saves it in your current directory. The -O option instructs curl to save the file with its original name.

After downloading, you can load the FPGA image onto your bladeRF device using the bladeRF-cli tool:

```
bladeRF-cli --load-fpga hostedxA4-latest.rbf
```
> Returns
```powershell
Loading FPGA...
[INFO @ /privatehost/libraries/libbladeRF/src/helpers/version.c:106] FPGA version (v0.15.3) is newer than entries in libbladeRF's compatibility table. Please update libbladeRF if problems arise.
Successfully loaded FPGA bitstream!
```

This command loads the FPGA image into the bladeRF device, preparing it for operation. ￼

To download the `adsbxA4.rbf` FPGA bitstream file for the bladeRF 2.0 micro xA4 using curl, execute the following command in your terminal:

```
curl -O https://www.nuand.com/fpga/adsbxA4.rbf
```
> Returns
```powershell
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
100 2570k    0 2570k    0     0   767k      0 --:--:--  0:00:03 --:--:--  767k
```

This command retrieves the `adsbxA4.rbf` file from the specified URL and saves it in your current directory. The -O option instructs curl to save the file with its original name.

After downloading, you can load the FPGA image onto your bladeRF device using the bladeRF-cli tool:

```
 bladeRF-cli --load-fpga adsbxA4.rbf
```
> Returns
```powershell
Loading FPGA...
Successfully loaded FPGA bitstream!
```

This command loads the FPGA image into the bladeRF device, preparing it for operation. ￼

## Version

```
bladeRF-cli --exec version
```
> Returns
```powershell

  bladeRF-cli version:        1.9.0-git-41ef6346-dirty
  libbladeRF version:         2.5.0-git-41ef6346-dirty

  Firmware version:           2.4.0-git-a3d5c55f
  FPGA version:               0.11.1 (configured by USB host)
```

# References

The `bladeRF-cli` is a command-line interface tool for interacting with the bladeRF Software Defined Radio. It allows users to perform tasks like updating firmware, loading FPGA bitstreams, configuring the radio, and running diagnostics.

Here is a guide to using `bladeRF-cli`:

---

### **General Syntax**
```bash
bladeRF-cli [options] [commands]
```

### **Common Tasks**

#### **1. Launch the CLI**
To start the interactive mode:
```bash
bladeRF-cli
```

Once inside, you can type commands interactively. Use `help` for a list of available commands.

#### **2. Display Device Information**
To view details about your bladeRF device:
```bash
bladeRF-cli -i
```
Or, from interactive mode:
```bash
info
```

#### **3. Load an FPGA Bitstream**
To load an FPGA bitstream onto the device:
```bash
bladeRF-cli -l <path_to_bitstream.rbf>
```
Example:
```bash
bladeRF-cli -l hostedxA4-latest.rbf
```

#### **4. Update Firmware**
To update the FX3 firmware:
```bash
bladeRF-cli -f <path_to_firmware.img>
```
Example:
```bash
bladeRF-cli -f bladerf_fw_v2.3.1.img
```

#### **5. Configure Frequencies**
Set the RX and TX frequencies:
```bash
set frequency rx <frequency_in_hz>
set frequency tx <frequency_in_hz>
```
Example:
```bash
set frequency rx 915000000  # 915 MHz
set frequency tx 2400000000 # 2.4 GHz
```

#### **6. Configure Gains**
Set RX and TX gains:
```bash
set gain rx <gain_value>
set gain tx <gain_value>
```
Example:
```bash
set gain rx 30  # Set RX gain to 30
set gain tx 20  # Set TX gain to 20
```

#### **7. Run Transceive or Receive**
Start receiving or transmitting data:
```bash
rx config file=<file> format=<format>
tx config file=<file> format=<format>
```
Supported formats include `sc16q11` and `csv`.

#### **8. Reset the Device**
To reset the bladeRF:
```bash
bladeRF-cli -r
```

#### **9. Execute a Script**
Run a predefined script containing bladeRF CLI commands:
```bash
bladeRF-cli -s <script_file>
```
Example:
```bash
bladeRF-cli -s config_script.txt
```

#### **10. Test Device**
Run diagnostic tests to verify the bladeRF's functionality:
```bash
bladeRF-cli -t
```

---

### **Help and Documentation**
To see the full list of commands and options, use:
```bash
bladeRF-cli -h
```
Or, in interactive mode:
```bash
help
```

This should cover most common use cases for the `bladeRF-cli` tool!
