# bladeRF


### bladeRF CLI

```
sudo bladeRF-cli -i
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
