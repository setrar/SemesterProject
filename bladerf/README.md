# bladeRF


### bladeRF CLI

```
sudo bladeRF-cli --interactive
```
> Returns
```powershell
[WARNING @ host/libraries/libbladeRF/src/board/bladerf2/bladerf2.c:461] FPGA bitstream file not found.
[WARNING @ host/libraries/libbladeRF/src/board/bladerf2/bladerf2.c:462] Skipping further initialization...
bladeRF>
```

# References

### nee sudo

```
bladeRF-cli -i
```
> Returns
```powershell
[WARNING @ host/libraries/libbladeRF/src/backend/usb/libusb.c:529] Found a bladeRF via VID/PID, but could not open it due to insufficient permissions.

No bladeRF device(s) available.

If one is attached, ensure it is not in use by another program
and that the current user has permission to access it.

bladeRF>
```


# References

#### Help

```
bladeRF-cli --help
```
> Returns
```powershell
Usage: bladeRF-cli <options>
bladeRF command line interface and test utility (1.9.0-git-fe3304d7)

Options:
  -d, --device <device>            Use the specified bladeRF device.
  -f, --flash-firmware <file>      Write the provided FX3 firmware file to flash.
  -l, --load-fpga <file>           Load the provided FPGA bitstream.
  -L, --flash-fpga <file>          Write the provided FPGA image to flash for
                                   autoloading. Use -L X or --flash-fpga X to
                                   disable FPGA autoloading.
  -p, --probe                      Probe for devices, print results, then exit.
                                    A non-zero return status will be returned if no
                                    devices are available.
  -e, --exec <command>             Execute the specified interactive mode command.
                                   Multiple -e flags may be specified. The commands
                                   will be executed in the provided order.
  -s, --script <file>              Run provided script.
  -i, --interactive                Enter interactive mode.
      --lib-version                Print libbladeRF version and exit.
  -v, --verbosity <level>          Set the libbladeRF verbosity level.
                                   Levels, listed in increasing verbosity, are:
                                    critical, error, warning,
                                    info, debug, verbose
      --version                    Print CLI version and exit.
  -h, --help                       Show this help text.
      --help-interactive           Print help information for all interactive
                                   commands.

Notes:
  The -d option takes a device specifier string. See the bladerf_open()
  documentation for more information about the format of this string.

  If the -d parameter is not provided, the first available device
  will be used for the provided command, or will be opened prior
  to entering interactive mode.

  Commands are executed in the following order:
    Command line options, -e <command>, script commands, interactive mode commands.

  When running 'rx/tx start' from a script or via -e, ensure these commands
  are later followed by 'rx/tx wait [timeout]' to ensure the program will
  not attempt to exit before reception/transmission is complete
```
