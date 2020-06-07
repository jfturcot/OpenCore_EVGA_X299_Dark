# OpenCore EFI for EVGA X299 Dark

My system configuration:

* CPU: 7920X
* GPU: AMD Vega 64

If you wish to use my EFI, make sure you update TSCAdjustReset.kext to your CPU's number of threads. My CPU is a 12 core/24 thread, so I have the following:

EFI/OC/Kexts/TSCAdjustReset.kext/Contents/Info.plist:
``
<dict>
  <key>IOCPUNumber</key>
  <integer>23</integer>
</dict>
``

Also don't forget to set your own serial numbers within the config.plist file.
