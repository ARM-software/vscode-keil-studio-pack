# Arm Keil Studio Pack for Visual Studio Code for the Web

## Overview

The **Keil Studio Pack For Web** installs recommended extensions for embedded and IoT software development on Arm-based microcontroller (MCU) devices. The extensions included are listed in the **Details** of the pack in Visual Studio Code and detailed in the [Extensions available in the pack](#extensions-available-in-the-pack) section below. 

The main Keil Studio extensions available with this pack are **Arm Device Manager** and **Arm Embedded Debugger**. The extensions can be used together by installing this pack, enabling you to run projects on a device and undertake debugging. Each extension can also be used individually.

This Readme explains how to install the extensions with the **Keil Studio Pack For Web**.

### Intended use cases

- **Embedded software development using CMSIS-Packs and csolution projects**: The "Common Microcontroller Software Interface Standard" (CMSIS) provides driver, peripheral and middleware support for thousands of MCUs and hundreds of development boards. Using the csolution project format, you can incorporate any CMSIS-Pack software component into your application. For more information about supported hardware for CMSIS projects, go to [keil.arm.com](https://www.keil.arm.com/boards/). For an overview on CMSIS-Packs, go to [open-cmsis-pack.org](https://www.open-cmsis-pack.org/index.html).
- **Enhancement of a pre-existing Visual Studio Code embedded software development workflow**: USB device management and embedded debug can be adapted to other project formats (for example CMake) and toolchains without additional overhead. This use case requires familiarity with Visual Studio Code to configure tasks. See the individual extensions for more details.

## Submit feedback

To submit feedback, please [create an issue](https://github.com/Arm-Software/vscode-keil-studio-pack/issues/new/choose).

## Table of contents

1. [Extensions available in the pack](#extensions-available-in-the-pack)
1. [Install the extensions](#install-the-extensions)

## Extensions available in the pack

The main extensions available are:

- **Arm Device Manager** (Identifier: `arm.device-manager`): This extension allows you to manage device connections for Arm Cortex-M based microcontrollers, development boards and debug probes.

- **Arm Embedded Debugger** (Identifier: `arm.embedded-debug`): This extension allows you to do flashing and debugging on Arm Cortex-M based microcontrollers, development boards and debug probes implementing the Microsoft Debug Adapter Protocol (DAP).

- **Arm Remote Build** (Identifier: `arm.remote-build`): This extension allows you to undertake remote builds of projects for Arm Cortex-M based microcontrollers. The extension only works with standalone CMSIS projects (containing a single `.cprj` project file). A token is required to access the service.

## Install the extensions

1. Go to the **Extensions** view.

1. Search for **Keil Studio Pack For Web**.

1. Click the **Install** button for the extension pack.

    Visual Studio Code installs the extensions. All recommended extensions are now available in the **Extensions** view.
