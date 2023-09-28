# Arm Keil Studio Pack for Visual Studio Code

## Overview

The **Keil Studio Pack** installs recommended extensions for embedded and IoT software development on Arm-based microcontroller (MCU) devices. The extensions included are listed in the **Details** of the pack in Visual Studio Code and described in [Extensions available in the pack](#extensions-available-in-the-pack).

We recommend installing the **Keil Studio Pack** in Visual Studio Code desktop to quickly set up your environment and start working with an example.

The main Keil Studio extensions available with the pack are **Arm CMSIS csolution**, **Arm Device Manager** and **Arm Embedded Debugger**. The extensions enable you to manage CMSIS solutions (csolution projects), run projects on a hardware and undertake debugging. The extensions can be used together or individually.

**Note**: The **Arm CMSIS csolution** and **Arm Environment Manager** extensions are not supported in Visual Studio Code for the Web.

This Readme explains how to install the extensions with Visual Studio Code desktop. When you have installed the pack, read the documentation available on Arm Developer to [get started with an example project](https://developer.arm.com/documentation/108029/latest/Get-started-with-an-example-project).

## Extensions available in the pack

The extensions available are:

- **Arm CMSIS csolution** (Identifier: `arm.cmsis-csolution`): This extension provides support for working with CMSIS solutions (csolution projects).

- **Arm Device Manager** (Identifier: `arm.device-manager`): This extension allows you to manage hardware connections for Arm Cortex-M based microcontrollers, development boards and debug probes.

- **Arm Embedded Debugger** (Identifier: `arm.embedded-debug`): This extension allows you to run and debug projects on Arm Cortex-M based microcontrollers, development boards and debug probes implementing the Microsoft Debug Adapter Protocol (DAP).

- **Arm Environment Manager** (Identifier: `arm.environment-manager`): This extension installs the tools you specify in a manifest file in your environment. For example, Arm Compiler for Embedded, CMSIS-Toolbox, CMake, and Ninja can be installed to work with CMSIS solutions.

- **Arm Remote Build** (Identifier: `arm.remote-build`): This extension allows you to undertake remote builds of projects for Arm Cortex-M based microcontrollers. The extension only works with standalone CMSIS projects (containing a single `.cprj` project file). An authentication token is required to access the service.

- **Arm Virtual Hardware** (Identifier: `arm.virtual-hardware`): This extension allows you to manage Arm Virtual Hardware and run embedded applications on them. An authentication token is required to access the service.

**Note**: The **Arm Remote Build** and **Arm Virtual Hardware** extensions are experimental.

The pack also installs:

- **Red Hat YAML** (Identifier: `redhat.vscode-yaml`): This extension provides YAML syntax support when editing `csolution.yml` or `cproject.yml` files.

- **Microsoft C/C++** (Identifier: `ms-vscode.cpptools`): This extension adds smart features such as code completion, compile errors, go-to-definition and more to your editor.

- **Microsoft C/C++ Themes** (Identifier: `ms-vscode.cpptools-themes`): This extension works in combination with **Microsoft C/C++** to provide syntax highlighting.

## Intended use cases for the extensions

- **Embedded and IoT software development using CMSIS-Packs and csolution projects**: The "Common Microcontroller Software Interface Standard" (CMSIS) provides driver, peripheral and middleware support for thousands of MCUs and hundreds of development boards. Using the csolution project format, you can incorporate any CMSIS-Pack based device, board, and software component into your application. For more information about supported hardware for CMSIS projects, go to the [Boards](https://www.keil.arm.com/boards/) and [Devices](https://www.keil.arm.com/devices/) pages on keil.arm.com. For information about CMSIS-Packs, go to [open-cmsis-pack.org](https://www.open-cmsis-pack.org/index.html).

- **Enhancement of a pre-existing Visual Studio Code embedded software development workflow**: USB device management and embedded debug can be adapted to other project formats (for example CMake) and toolchains without additional overhead. This use case requires familiarity with Visual Studio Code to configure tasks. See the individual extensions for more details.

## Install the extensions

1. In Visual Studio Code desktop, go to the **Extensions** view.

1. Search for **Keil Studio Pack**.

1. Click the **Install** button for the extension pack.

    Visual Studio Code installs the extensions.
    All recommended Keil Studio extensions are now available in the **Extensions** view, including the  **Arm Environment Manager**. The pack also installs the **Red Hat YAML**, **Microsoft C/C++**, and **Microsoft C/C++ Themes** extensions.

    A pop up displays in the bottom right-hand corner with the message "Activate license for Arm tools?". See [Activate your license to use Arm tools](https://developer.arm.com/documentation/108029/latest/Activate-your-license-to-use-Arm-tools) for more details on licensing.

1. Click **Activate**.

## Submit feedback

To submit feedback, please [see our support page](https://www.keil.arm.com/support/#:~:text=Keil%20Studio%20for%20VS%20Code).