# Arm Keil Studio Pack for Visual Studio Code for the Web

## Overview

This Readme explains how to install the extensions with the **Keil Studio Pack For Web**.

The **Keil Studio Pack For Web** installs recommended extensions for embedded and IoT software development on Arm-based microcontroller (MCU) devices. The extensions included are listed in the **Details** of the pack in Visual Studio Code and detailed in the [Extensions available in the pack](#extensions-available-in-the-pack) section below. 

The main Keil Studio extensions available with this pack are **Arm Device Manager** and **Arm Embedded Debugger**. The extensions can be used together by installing this pack, enabling you to run projects on a hardware and undertake debugging. Each extension can also be used individually.

## Extensions available in the pack

The main extensions available are:

- **Arm Device Manager** (Identifier: `arm.device-manager`): This extension allows you to manage hardware connections for Arm Cortex-M based microcontrollers, development boards and debug probes.

- **Arm Embedded Debugger** (Identifier: `arm.embedded-debug`): This extension allows you to run and debug projects on Arm Cortex-M based microcontrollers, development boards and debug probes implementing the Microsoft Debug Adapter Protocol (DAP).

- **Arm Remote Build** (Identifier: `arm.remote-build`): This extension allows you to undertake remote builds of projects for Arm Cortex-M based microcontrollers. The extension only works with standalone CMSIS projects (containing a single `.cprj` project file). An authentication token is required to access the service.

- **Arm Virtual Hardware** (Identifier: `arm.virtual-hardware`): This extension allows you to manage Arm Virtual Hardware and run embedded applications on them. An authentication token is required to access the service.

**Note**: The **Arm Remote Build** and **Arm Virtual Hardware** extensions are experimental.

## Intended use cases for the extensions

- **Embedded and IoT software development using CMSIS-Packs and csolution projects**: The "Common Microcontroller Software Interface Standard" (CMSIS) provides driver, peripheral and middleware support for thousands of MCUs and hundreds of development boards. Using the csolution project format, you can incorporate any CMSIS-Pack based device, board, and software component into your application. For more information about supported hardware for CMSIS projects, go to the [Boards](https://www.keil.arm.com/boards/) and [Devices](https://www.keil.arm.com/devices/) pages on keil.arm.com. For information about CMSIS-Packs, go to [open-cmsis-pack.org](https://www.open-cmsis-pack.org/index.html).

- **Enhancement of a pre-existing Visual Studio Code embedded software development workflow**: USB device management and embedded debug can be adapted to other project formats (for example CMake) and toolchains without additional overhead. This use case requires familiarity with Visual Studio Code to configure tasks. See the individual extensions for more details.

## Install the extensions

1. Go to the **Extensions** view.

1. Search for **Keil Studio Pack For Web**.

1. Click the **Install** button for the extension pack.

    Visual Studio Code installs the extensions. All recommended extensions are now available in the **Extensions** view.

## Submit feedback

To submit feedback, please [open a bug report or a feature request](https://github.com/Arm-Software/vscode-keil-studio-pack/issues/new/choose).
