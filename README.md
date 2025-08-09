# Curated overview of consumer SBC (single board computers) that are interesting

This is not a comprehensive list, mainly ARM based SBCs. Hopefully at some point, they will be added to this (a bit outdated) list: https://en.wikipedia.org/wiki/User:OliverGalvin/Comparison_of_single-board_computers
For many comprehensive reviews and benchmark see review by Jeff Geerling: https://sbc-reviews.jeffgeerling.com/

# SBCs
| Make | Model | Soc | RAM size | Storage | Notes | Review | Price (per RAM version) |
| --- | --- | --- | --- | --- | --- | --- | --- |
| Raspberry Pi | [Zero 2 W](https://www.raspberrypi.com/products/raspberry-pi-zero-2-w/) | BCM2710A1 | 512 MB | microSD | | [by Jeff Geerling](https://github.com/geerlingguy/sbc-reviews/issues/43) | 24 EUR |
| Luckfox | [Lyra Zero W](https://www.luckfox.com/Luckfox-Lyra-Zero-W) | RK3506B | 512 MB | 256 MB flash/microSD | | | 25 EUR |
| Orange Pi | [Zero 2W](http://www.orangepi.org/html/hardWare/computerAndMicrocontrollers/details/Orange-Pi-Zero-2W.html) | H618 | 1/2/4 GB | microSD | | [by Jeff Geerling](https://www.jeffgeerling.com/blog/2021/look-inside-raspberry-pi-zero-2-w-and-rp3a0-au) | 32/45/. Eur |
| Orange Pi | [3 LTS](http://www.orangepi.org/orangepiwiki/index.php/Orange_Pi_3_LTS) | H6 | 2 GB | eMMC 8GB/microSD | | | 61 EUR |
| Orange Pi | [3b](http://www.orangepi.org/html/hardWare/computerAndMicrocontrollers/details/Orange-Pi-3B.html) | RK3566 | 2/4/8 GB | eMMC socket/microSD | | | 51/___/___ GB |
| Orange Pi | [4b](http://www.orangepi.org/html/hardWare/computerAndMicrocontrollers/details/orange-pi-4B.html) | RK3399 | 2/8/16 GB | eMMC/microSD | | | |
| Banana Pi | [M5](https://wiki.banana-pi.org/Banana_Pi_BPI-M5) | S905X3 | 4GB | 16GB eMMC/microSD | Not available | | |
| Radxa | [ROCK 5C](https://radxa.com/products/rock5/5c/) | RK3588S2 | 2/8/16 GB | SDcard/eMMC socket | NPU | [by Jeff Geerling](https://github.com/geerlingguy/sbc-reviews/issues/41) | 89/102/136 EUR |
| Radxa | [ROCK 5C Lite](https://radxa.com/products/rock5/5c/) | RK3582 | 2/8/16 GB | SDcard/eMMC socket | | | 85/___/___ EUR |
| Raspbery Pi | [5](https://www.raspberrypi.com/products/raspberry-pi-5/) | BCM2712 | 4/8 GB | microSD | | [by Jeff Geerling](https://github.com/geerlingguy/sbc-reviews/issues/21) | ___/80 EUR |
| Radxa X4 | [X4](https://radxa.com/products/x/x4/) | N100 | 4/8/12/16 GB | m.2(42mm) | | [by Jeff Geerling](https://www.jeffgeerling.com/blog/2024/radxa-x4-sbc-unites-intel-n100-and-raspberry-pi-rp2040) | 70/93/114/130 EUR |


# Processors

| Name | Cores | RAM type | Freq | GPU | Notes |
| --- | --- | --- | --- | --- | --- |
| [Rockchip](https://en.wikipedia.org/wiki/List_of_Rockchip_products) [RK3588](https://www.rockchips.net/product/rk3588/) (S, S2)[^2] | 4x A76, 4x A55 |  |  | Mali-G610 MC4 | 3x core NPU[^1] [^3] |
| Rockchip [RK3399](https://opensource.rock-chips.com/wiki_RK3399) |2 x A72, 4x A53 | DDR3/4 LPDDR3/4 | | Mali-T864 |  |
| Rockchip [RK3582](https://www.cnx-software.com/2024/03/25/rockchip-rk3582-is-a-cost-down-version-of-rk3588s-with-two-cortex-a76-cores-four-cortex-a55-cores-no-gpu/) | 2x A76, 4x A55 | LPDDR4/LPDDR4x/LPDDR5 | | Mali-G610 MC4 (no 3D) | |
| Rockchip [RK3506B](https://www.cnx-software.com/2023/11/02/rockchip-roadmap-reveals-rk3576-and-rk3506-iot-processors-linux-6-1-sdk/) | 3x A7, 1x M0 | DDR3 | 1.2 GHz | Mali G52 | |
| Broadcom [BCM2710A1](https://datasheets.raspberrypi.com/rpizero2/raspberry-pi-zero-2-w-product-brief.pdf) | 4x A53 | LPDDR2 | | VideoCore IV |  |
| Broadcom [BCM2712](https://www.notebookcheck.net/Broadcom-BCM2712-Processor-Benchmarks-and-Specs.873280.0.html) | 4x A76 | LPDDR4X | | VideoCore V3D VII | | 
| [Allwinner](https://linux-sunxi.org/Allwinner_SoC_Family) [H618](https://linux-sunxi.org/H618) | 4x A53 | DDR3/4 LPDDR3/4 | | Mali-G31 MP2| |
| Allwinner [H6](https://linux-sunxi.org/H6) | 4x A53 | DDR2/3 LPDDR3/4 | | Mali-T720 MP2 | |
| Allwinner [A64](https://www.cnx-software.com/2015/11/10/allwinner-a64-datasheet-and-user-manual-released/) | 4x A53 | DDR2/3 LPDDR2/3 | | Mali-400 MP2 | Outdated |
| Intel [N100](https://www.intel.com/content/www/us/en/products/sku/231803/intel-processor-n100-6m-cache-up-to-3-40-ghz/specifications.html) | 4x Alder Lake-N | LPDDR4/5 | 3.4 GHz |  | x86-64bit |
| NXP [i.MX 8M](https://www.nxp.com/products/i.MX8M) | 4x A53, 1x M4F| DDR3/4 LPDDR4 | | Vivante GC7000-Lite | |
| Amlogic [S905X3](https://www.cnx-software.com/2019/04/12/amlogic-s905x3-specifications-block-diagram/) | 4x A55 | DDR3/4 LPDDR3/4 | | Mali G31 MP2  | |


# Cores

| Name | ISA |
| --- | --- |
| [Cortext M](https://www.arm.com/products/silicon-ip-cpu/cortex-m/cortex-m0) | Armv6-M |
| [Cortex A7](https://www.arm.com/products/silicon-ip-cpu/cortex-a/cortex-a7) | Armv7 |
| [Cortex A53](https://developer.arm.com/Processors/Cortex-A53) | Armv8-A |
| [Cortex A55](https://developer.arm.com/Processors/Cortex-A55) | Armv8-A |
| [Cortex A72](https://developer.arm.com/Processors/Cortex-A72) | Armv8-A |
| [Cortex A76](https://developer.arm.com/Processors/Cortex-A76) | Armv8-A |
| [Alder Lake-N](https://en.wikipedia.org/wiki/Alder_Lake#Alder_Lake-N) | x86-64bit |


# Storage
microSD = has a slot for microSD card, needs to be bought extra
eMMC = has on-board soldered eMMC (optionally)
eMMC socket = has a socket for external eMMC board, needs to be bought extra

Some boards have eMMC storage directly on-board. These boards look more expensive but you don't need to buy the microSD card.
Socketted eMMC is about 64GB for 20 EUR and 256 for 45 EUR
microSD Samsung EVO A2 256 is 20 EUR
m.2 (42mm) 256GB is 40 EUR

# More power
For more powerful computer systems look at the Intel N100, N150, N200 line

# Nvidia boards
At this moment, I do not recommend these boards for commercial use, due to their poor bringup software (Installation wizard), poor documentation, poor support on forums and poor supplly chain security.
A good overview is on [Wikipedia](https://en.wikipedia.org/wiki/Nvidia_Jetson#Performance)

Generations:
TK1, TX1, Nano = long obsolete [Maxwell](https://en.wikipedia.org/wiki/Maxwell_(microarchitecture)) (2014, 2015)
TX2 = obsolete [Pascal](https://en.wikipedia.org/wiki/Pascal_(microarchitecture)) (2016)
Xavier = [Volta microachitecture](https://en.wikipedia.org/wiki/Volta_(microarchitecture)) (2017)
Orin = [Ampere microachitecture](https://en.wikipedia.org/wiki/Ampere_(microarchitecture)) (2020)
Thor = [Blackwell microachitecture](https://en.wikipedia.org/wiki/Blackwell_(microarchitecture)) (2024)

Form factors:
Nano, NX = SoDIMM modules[^8] usable with the Dev-Kit board
AGX = SoM with 699-pin Moles connector[^9]

## Nano
The starter board everyone usually knows is the _Jetson Nano_ (now obsolete), and its newer variants _Orin Nano_ and _Orin Nano Super_. ~15W TDP
The compute module (Tegra SoC and friends) is in a form of a DIMM module that's usually on a motherboard ("devkit") with all the peripherals broken out.
Orin Nano and Orin NX and Xavier NX are mostly compatible.[^4]
The versions with less memory may also have less CUDA and tensor cores and slower memory.[^5]
Other funny stuff may include things such ass; the Orin Nano USB3 ports are internally connected to a USB2 hub. USB3 could theoretically be brought out via m.2 PCIe.
Orin Nano has no HW video encoder except JPEG.
GPIO pin mapping is complicated and may need a reconfiguration via device-tree overlay generated by a official Office Spreadsheet file (which hangs LibreOffice).
The USBC port acts as a Ethernet-over-USB port and works on 192.168.55.0/24 address space. Peer IPs are 1 and 100

## Xavier
Xavier NX (20W TDP) and higher spec Xavier AGX (30W TDP).[^6]

## AGX
Higher power boards such as Jetson AGX Xavier have a different form factor from the Nanos.
To compare modules, view this [overview](https://www.nvidia.com/en-us/autonomous-machines/embedded-systems/jetson-xavier-series/) or this [disgusting modal](https://www.nvidia.com/en-us/autonomous-machines/embedded-systems/jetson-agx-xavier/#agx-xavier-series-compare).

## Thor
Upcoming (2025) series. Marketing says 2000 TFLOPS \* 4bit \*\* sparse, so divide it by a factor of two and then another factor of two, 75-130W TDP.[^7]

# Hire me
For consultations, schedule a call via _Calendly_ link in my profile.


References:
[^1]: https://clehaxze.tw/gemlog/2024/02-14-benchmarking-rk3588-npu-matrix-multiplcation-performance-ep2.gmi
[^2]: S and S2 variants are just binned to a lower spec: https://www.rockchips.net/rk3588-vs-rk3588s-in-depth-technical-comparison/
[^3]: https://clehaxze.tw/gemlog/2023/07-13-rockchip-npus-and-deploying-scikit-learn-models-on-them.gmi
[^4]: https://developer.download.nvidia.com/assets/embedded/secure/jetson/orin_nano/docs/Jetson_OrinNano_OrinNX_XavierNX_Interface_Comparison_Migration_DA-11081-001_v1.1.pdf
[^5]: https://www.seeedstudio.com/blog/nvidia-jetson-comparison-nano-tx2-nx-xavier-nx-agx-orin/
[^6]: https://www.nvidia.com/en-us/autonomous-machines/embedded-systems/jetson-xavier-series/
[^7]: https://www.nvidia.com/en-us/autonomous-machines/embedded-systems/jetson-thor/
[^8]: https://developer.download.nvidia.com/assets/embedded/secure/jetson/docs/Ruggedized_Systems_with_Jetson_SoDIMM_Modules_TB-10728-001-v1.1.pdf
[^9]: https://www.molex.com/en-us/products/part-detail/2034560003
