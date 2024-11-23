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
