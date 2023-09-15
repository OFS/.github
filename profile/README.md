# **Open FPGA Stack Overview**

<img src="https://github.com/OFS/ofs.github.io/blob/main/docs/hw/n6001/reference_manuals/ofs_fim/images/ofs-logo-1x1.png" align="right" width="150" height="150">

 Open FPGA Stack (OFS) is an open-source solution that provides a hardware and software framework for building your shell design and subsequently your workload.  
OFS provides reference shell designs targeting different Intel<sup>&reg;</sup> FPGA devices with upstreamed drivers and management software tools.  

<br>

## **Open FPGA Stack Repositories**

Accessing OFS ingredients to use within the development framework is easy.  The github.com/OFS site provides all the hardware and software repositories in one location.

|Development Focus|Repository Folder | Description |
|:----------------:|:------------------:|:--------------------|
|Hardware | [ofs-agx7-pcie-attach](https://github.com/OFS/ofs-n6001) | Provides RTL, unit tests, and build scripts to create an example Intel<sup>&reg;</sup> Agilex<sup>&reg;</sup> 7 FIM and is leveraged as a starting point for a custom PCIe Attach design.  The reference FIM targets both the [Intel® FPGA SmartNIC N6001-PL Platform](https://www.intel.com/content/www/us/en/products/details/fpga/platforms/smartnic/n6000-pl-platform.html) and [Intel Agilex 7 FPGA F-Series Development Kit (2x F-Tile) User Guide](https://www.intel.com/content/www/us/en/docs/programmable/739942/current/overview.html). |
|Hardware | [ofs-f2000x-pl](https://github.com/OFS/ofs-f2000x-pl) | Provides RTL, unit tests, and build scripts to create an example Intel<sup>&reg;</sup> Agilex<sup>&reg;</sup> 7 FIM and is leveraged as a starting point for a custom SoC Attach design.  The reference FIM targets an [Intel® FPGA IPU F2000X-PL Platform](https://www.intel.com/content/www/us/en/products/details/network-io/ipu/f2000x-pl-platform.html). |
|Hardware | [ofs-d5005](https://github.com/OFS/ofs-d5005) | Provides RTL, unit tests, and build scripts to create an example Intel<sup>&reg;</sup> Stratix 10<sup>&reg;</sup> FIM and is leveraged as a starting point for a custom PCIe Attach design.  The reference FIM targets an Intel® FPGA PAC D5005 development board. |
| Hardware| [oneapi-asp](https://github.com/OFS/oneapi-asp) | Contains the files to generate the support package that works with the reference shells and allows you to use OneAPI. This is an optional repository for developers interested in OneAPI|
|Hardware| [ofs-fim-common](https://github.com/OFS/ofs-fim-common) | Provides RTL components that are shared among all new platforms that are introduced in OFS.  This folder is a subumodule in each platform repository folder. |
| Hardware | [examples-afu](https://github.com/OFS/examples-afu) | Provides simple Accelerator Functional Unit (AFU) examples you can use as a template for starting your own workload design.  |
| Hardware | [ofs-platform-afu-bbb](https://github.com/OFS/ofs-platform-afu-bbb) | Contains the hardware code to build a standard interface between the FIM and your workload. | 
| Software | [linux-dfl](https://github.com/OFS/linux-dfl) | This repository is a mirror of the linux.org Git site and contains the most up-to-date drivers that are being developed and upstreamed for OFS platforms.|
| Software | [meta-ofs](https://github.com/OFS/meta-ofs) | This repository provides the Linux<sup>&reg;</sup> DFL kernel and the OPAE SDK for the Yocto<sup>&reg;</sup> Project.|
| Software | [opae-sdk](https://github.com/OFS/opae-sdk) | Contains the ingredients to build the OFS Open Programmable Acceleration Engine (OPAE) Software Development Kit which provides APIs and userspace tools for OFS FPGA management. |
| Software | [opae-sim](https://github.com/OFS/opae-sim) | This repository is used to build the AFU Hardware/Software Co-Simulation Environment workload developers can use to ensure their AFU can work with the OFS software stack. |
| Software | [linux-dfl-backport](https://github.com/OFS/linux-dfl-backport) | A place for finding and leveraging out-of-tree backported drivers for older OS versions .  |
| Software | [opae-legacy](https://github.com/OFS/opae-legacy) | Supports OFS platforms built on the legacy version of OPAE software.  Not used in current OFS designs |
| Documentation | [ofs.github.io](https://github.com/OFS/ofs.github.io) | Contains the hardware and software collateral that surfaces on the OFS website: <https://ofs.github.io> | 

<br/>
<br/>

## **How Can I Start Using OFS?**

To find out how easy it is to use OFS for your custom applications, please go to https://ofs.github.io/.

To find information on the latest releases, go to the [Discussions Tab](https://github.com/orgs/OFS/discussions) in the OFS GitHub repository.




