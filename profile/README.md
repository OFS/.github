# **Open FPGA Stack Overview**

<img src="https://github.com/OFS/ofs.github.io/blob/main/docs/hw/d5005/reference_manuals/ofs_fim/images/OFS.png" align="right" width="150" height="150">

 Open FPGA Stack (OFS) is an open-source solution that provides a hardware and software framework for building your shell design and subsequently your workload.  
OFS provides reference shell designs targeting different Intel<sup>&reg;</sup> FPGA devices with upstreamed drivers and management software tools.  

<br>

## **Open FPGA Stack Repositories**

Accessing OFS ingredients to use within the development framework is easy.  The github.com/OFS site provides all the hardware and software repositories in one location.

|Development Focus|Repository Folder | Description |
|:----------------:|:------------------:|:--------------------|
|Hardware | [ofs-d5005](https://github.com/OFS/ofs-d5005) | Provides RTL, unit tests, and build scripts to create Intel<sup>&reg;</sup> Stratix<sup>&reg;</sup> 10 FIM and is leveraged as a starting point for a custom design.  The reference FIM targets an Intel FPGA PAC D5005 development board. |
|Hardware| [ofs-fim-common](https://github.com/OFS/ofs-fim-common) | Provides RTL components that are shared among all new platforms that are introduced in OFS.  This folder is a subumodule in each platform repository folder. |
| Hardware | [examples-afu](https://github.com/OFS/examples-afu) | Provides simple Accelerator Functional Unit (AFU) examples you can use as a template for starting your own workload design.  |
| Hardware | [ofs-platform-afu-bbb](https://github.com/OFS/ofs-platform-afu-bbb) | Contains the hardware code to build a standard interface between the FIM and your workload. | 
| Software | [linux-dfl](https://github.com/OFS/linux-dfl) | This repository is a mirror of the linux.org Git site and contains the most up-to-date drivers that are being developed and upstreamed for OFS platforms.|
| Software | [opae-sdk](https://github.com/OFS/opae-sdk) | Contains the ingredients to build the OFS Open Programmable Acceleration Engine (OPAE) Software Development Kit which provides APIs and userspace tools for OFS FPGA management. |
| Software | [opae-sim](https://github.com/OFS/opae-sim) | This repository is used to build the AFU Hardware/Software Co-Simulation Environment workload developers can use to ensure their AFU can work with the OFS software stack. |
| Software | [linux-dfl-backport](https://github.com/OFS/linux-dfl-backport) | A place for finding and leveraging out-of-tree backported drivers for older OS versions .  |
| Software | [opae-legacy](https://github.com/OFS/opae-legacy) | Supports OFS platforms built on the legacy version of OPAE software.  Not used in current OFS designs |
| Documentation | [ofs.github.io](https://github.com/OFS/ofs.github.io) | Contains the hardware and software collateral that surfaces on the OFS website: <https://ofs.github.io> | 

<br/>
<br/>

## **How Can I Start Using OFS?**

The best way to start using OFS is to evaluate the reference FIM that can be built in the platform repository by leveraging our evaluation scripts to run through the hardware and software build flow and test the design in simulation and optionally hardware as well.  We have step-by-step documentation to guide you through the evaluation and development process.

Click here for the [Intel Stratix 10 OFS Collateral](https://ofs.github.io/hw/d5005/user_guides/ug_eval_ofs_d5005/ug_eval_script_ofs_d5005/) to get started.

Our software development collateral is found at the same location [here](https://ofs.github.io/sw/fpga_api/quick_start/readme/).

The reference FIM in the platform repository currently targets PCIe attach applications and can be used as-is or can be used as a starting point for modification, greatly reducing development time. The ofs-d5005 repository provides capability to build an Intel Stratix 10 OFS reference FIM.  Additional repositories that support Intel Agilex FPGA will be introduced in a future OFS GitHub release.  For more information about our upcoming Intel Agilex releases, visit the OFS webpage on [intel.com](https://www.intel.com/content/www/us/en/products/details/fpga/platforms/pac/open-fpga-stack.html) and fill out our available questionnaire.

<image src="https://github.com/OFS/ofs.github.io/blob/main/docs/hw/d5005/reference_manuals/ofs_fim/images/FIM-s10-OFS block.png" align="center" width="750" height="750">

<br/>
<br/>


**OFS FIM Targeting Intel Stratix 10 FPGA**

| Key Feature | Intel Stratix 10 Reference FIM | 
|:-----------:|:-------------------------------|
|FPGA  | Intel Stratix 10 SX FPGA |
|Ethernet Configuration | 1x10GbE example with 2x100GbE capability |
| PCIe | Gen3x16 |
|EMIF | Up to four DDR channels |
| PF/VF | 1 PF/3 VFs |
|Management | FPGA Management Engine (FME) with FIM management registers|
|Interface | ARM<sup>&reg;</sup> AMBA<sup>&reg;</sup> AXI4 Interface|
| HLD support | oneAPI (coming soon!) |
| Software | Kernel code upstreamed to Linux.org |

Note: Source code for BMC RTL/Firmware that works with this reference FIM can be obtained by contacting your Intel Sales Representative.

To find information on the latest releases, go to the [Discussions Tab](https://github.com/orgs/OFS/discussions) in the OFS GitHub repository.




