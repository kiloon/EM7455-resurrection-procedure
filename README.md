# EM7455-resurrection-procedure
How to unbrick Sierra Wireless (DW5811e) EM7455
Do not install any drivers
Download following Driver Pack: [mega.nz/#!SYcBRR5S!KLBFTWvQ3cFK … 3LsXGcc3Ng 402](https://mega.nz/file/SYcBRR5S#KLBFTWvQ3cFK6CBiKQmVqwq_atl54wBEI3LsXGcc3Ng)
in Device Manager find the EM7455 device which Hardware-ID ends with “&MI_03” (its the Modem Device, “MI_03” always corresponds to the AT command COM port)
Update Driver > Browse my Computer > pick from a list of device drivers etc… > chose x86 or x64 directory and choose “Huawei Incorporated“ then “HUAWEI Mobile Broadband – Modem"
the Modem started and i could connect with putty on specified COM port !


now you can do the rest:
Open AT Port (with Putty or other program) and excute this commands:
AT!ENTERCND=“A710”
AT!USBPID=9071,9070
AT!USBVID=1199
AT!USBPRODUCT=“EM7455”
AT!PRIID=“9904802”,“001.001”,“Generic-Laptop”
AT!RESET
Install Sierra Wireless drivers.
