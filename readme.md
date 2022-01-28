# Samsung Galaxy S5 SM-G900H Kernel Source

Kernel Source 3.10.9 for the Samsung Galaxy S5 Exynos

---
![Samsung Galaxy S5](https://fdn2.gsmarena.com/vv/pics/samsung/samsung-galaxy-s5-g900f-1.jpg)


# About Device

Samsung Galaxy S5 Exynos (k3gxx)

### Specifications

Basic   | Spec Sheet
-------:|:-------------------------
CPU     | Octa-core 4x1.9GHz Cortex-A15 + 4x1.3Ghz Cortex-A7, ARM big.LITTLE
Chipset | Samsung Exynos 5422 Octa
GPU     | ARM Mali T628-MP6
Memory  | 2 GB
Shipped Android Version | 4.4.2
Updated Android Version | 6.0.1
Storage | 16 GB
MicroSD | Up to 64 GB
Battery | 2800 mAh (non-removable)
Dimensions | 159 x 75.1 x 8.5 mm
Display | 1080 x 1920 pixels, 5.1" Super AMOLED
Rear Camera  | 16.0 MP, LED Flash
Front Camera | 2.1 MP

---

#  Steps to Compile

Included arm-eabi-4.8 toolchain located in toolchain folder

Then add a build script or use the "build_s5.sh" script
example:
```sh
export ARCH=arm
export CROSS_COMPILE=path_to_toolchain_executables
make clean && make mrproper
make exynos5422-k3g_00_defconfig
make j#
```
'#'=no of CPU threads your CPU has.
```sh
./build_script_name.sh
```
### Thanks to:
 * myself
 * Samsung for providing kernel source

