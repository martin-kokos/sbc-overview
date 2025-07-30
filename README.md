# Curated overview of consumer SBC (single board computers) that are interesting

This is not a comprehensive list, mainly ARM based SBCs. Hopefully at some point, they will be added to this (a bit outdated) list: https://en.wikipedia.org/wiki/User:OliverGalvin/Comparison_of_single-board_computers
For many comprehensive reviews and benchmark see review by Jeff Geerling: https://sbc-reviews.jeffgeerling.com/

# SBCs
| Make | Model | Soc | RAM size | Storage | Notes | Review | Price (per RAM version) |
| --- | --- | --- | --- | --- | --- | --- | --- |
| Raspberry Pi | [Zero 2 W](https://www.raspberrypi.com/products/raspberry-pi-zero-2-w/) | BCM2710A1 | 512 MB | SDcard | | [by Jeff Geerling](https://github.com/geerlingguy/sbc-reviews/issues/43) | 24 EUR |
| Orange Pi | [Zero 2W](http://www.orangepi.org/html/hardWare/computerAndMicrocontrollers/details/Orange-Pi-Zero-2W.html) | H618 | 1/2/4 GB | microSD | | [by Jeff Geerling](https://www.jeffgeerling.com/blog/2021/look-inside-raspberry-pi-zero-2-w-and-rp3a0-au) | 32/45/. Eur |
| Orange Pi | [3 LTS](http://www.orangepi.org/orangepiwiki/index.php/Orange_Pi_3_LTS) | H6 | 2 GB | eMMC 8GB/microSD | | | 61 EUR |
| Orange Pi | [3b](http://www.orangepi.org/html/hardWare/computerAndMicrocontrollers/details/Orange-Pi-3B.html) | RK3566 | 2/4/8 GB | eMMC socket/microSD | | | 51/___/___ GB |
| Orange Pi | [4b](http://www.orangepi.org/html/hardWare/computerAndMicrocontrollers/details/orange-pi-4B.html) | RK3399 | 2/8/16 GB | eMMC/microSD | | | |
| Banana Pi | [M5](https://wiki.banana-pi.org/Banana_Pi_BPI-M5) | S905X3 | 4GB | 16GB eMMC/microSD | Not available | | |
| Radxa | [ROCK 5C](https://radxa.com/products/rock5/5c/) | RK3588S2 | 2/8/16 GB | SDcard/eMMC socket | | [by Jeff Geerling](https://github.com/geerlingguy/sbc-reviews/issues/41) | 89/102/136 EUR |
| Radxa | [ROCK 5C Lite](https://radxa.com/products/rock5/5c/) | RK3582 | 2/8/16 GB | SDcard/eMMC socket | | | 85/___/___ EUR |
| Raspbery Pi | [5](https://www.raspberrypi.com/products/raspberry-pi-5/) | BCM2712 | 4/8 GB | microSD | | [by Jeff Geerling](https://github.com/geerlingguy/sbc-reviews/issues/21) | ___/80 EUR |
| Radxa X4 | [X4](https://radxa.com/products/x/x4/) | N100 | 4/8/12/16 GB | m.2(42mm) | | [by Jeff Geerling](https://www.jeffgeerling.com/blog/2024/radxa-x4-sbc-unites-intel-n100-and-raspberry-pi-rp2040) | 70/93/114/130 EUR |


# Processors

| Name | Cores | RAM type | Freq | GPU | Notes |
| --- | --- | --- | --- | --- | --- |
| [Rockchip](https://en.wikipedia.org/wiki/List_of_Rockchip_products) [RK3588](https://www.rockchips.net/product/rk3588/) | 4x A76, 4x A55 |  |  | Mali-G610 MC4 | 3x NPU |
| Rockchip [RK3399](https://opensource.rock-chips.com/wiki_RK3399) |2x A72, 4x A53 | DDR3/4 LPDDR3/4 | | Mali-T864 |  |
| Rockchip [RK3582](https://www.cnx-software.com/2024/03/25/rockchip-rk3582-is-a-cost-down-version-of-rk3588s-with-two-cortex-a76-cores-four-cortex-a55-cores-no-gpu/) | 2x A76, 4x A55 | LPDDR4/LPDDR4x/LPDDR5 | | Mali-G610 MC4 (no 3D) | |
| Broadcom [BCM2710A1](https://datasheets.raspberrypi.com/rpizero2/raspberry-pi-zero-2-w-product-brief.pdf) | 4x A53 | LPDDR2 | | VideoCore IV |  |
| Broadcom [BCM2712](https://www.notebookcheck.net/Broadcom-BCM2712-Processor-Benchmarks-and-Specs.873280.0.html) | 4x A76 | LPDDR4X | | VideoCore V3D VII | | 
| [Allwinner](https://linux-sunxi.org/Allwinner_SoC_Family) [H618](https://linux-sunxi.org/H618) | 4x A53 | DDR3/4 LPDDR3/4 | | Mali-G31 MP2| |
| Allwinner [H6](https://linux-sunxi.org/H6) | 4x A53 | DDR2/3 LPDDR3/4 | | Mali-T720 MP2 | |
| Allwinner [A64](https://www.cnx-software.com/2015/11/10/allwinner-a64-datasheet-and-user-manual-released/) | 4x A53 | DDR2/3 LPDDR2/3 | | Mali-400 MP2 | Outdated |
| Intel [N100](https://www.intel.com/content/www/us/en/products/sku/231803/intel-processor-n100-6m-cache-up-to-3-40-ghz/specifications.html) | 4x Alder Lake-N | LPDDR4/5 | 3.4 GHz |  | x86-64bit |
| Amlogic [S905X3](https://www.cnx-software.com/2019/04/12/amlogic-s905x3-specifications-block-diagram/) | 4x A55 | DDR3/4 LPDDR3/4 | | Mali G31 MP2  | |


# Cores

| Name | ISA |
| --- | --- |
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
