# TWRP device tree for Tecno Camon 19 Neo (CH6i) - A12
MT6768 - Helio G85

## Status

Specs [here](https://www.gsmarena.com/tecno_camon_19_neo-11619.php)

## What's the history?
The tester [tommynok -4pda](https://4pda.to/forum/index.php?showuser=4408448) only install `boot-TECNO-CH6i_V1529-A12_noCrypt.img` test file to know if TWRP can start.

#### This branch A12 not have encrypt/decrypt process and files because boot.img has only 32MB. So is need change the `\vendor\etc\fstab.mt6768` to ***encryptable*** in the vendor.img for TWRP backup the `\Data` partition.

---------------------------

![Tecno Camon 19 Neo](https://fdn2.gsmarena.com/vv/pics/tecno/tecno-camon-19-neo-1.jpg)

---------------------------
                  ####### generated by lopestom #######
---------------------------
### TWRP
![Menu](https://github.com/lopestom/twrp_device_tecno_CH6i/releases/download/TECNO_Camon_19_Neo-CH6i/Screenshot_2023-04-09-19-57-54.png)

---------------
## Building

```bash
source build/envsetup.sh
lunch twrp_CH6i-eng
mka bootimage
```
-------------

