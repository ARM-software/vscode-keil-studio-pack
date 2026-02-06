# Keil Studio

Keil Studio is Arm's new IDE that brings powerful embedded development capabilities directly into Visual Studio Code. As the successor to the µVision IDE, Keil Studio represents a modern approach to embedded development, offering seamless integration with industry-standard tools, version control systems, and command line interface (CLI) for continuous integration (CI) workflows.

Being part of [Arm Keil MDK 6](https://www.keil.arm.com/), Keil Studio provides comprehensive support for Cortex-M based microcontrollers. It combines the reliability and maturity of the Arm Compiler and extensive device support, with the flexibility and extensibility of Visual Studio Code.

![Keil Studio](https://github.com/ARM-software/vscode-keil-studio-pack/raw/main/images/KeilStudio.png)

When using Keil Studio the [VS Code Activity Bar](https://code.visualstudio.com/docs/getstarted/getting-started#_switch-between-views-with-the-activity-bar) provides these views:

- The [CMSIS view](https://mdk-packs.github.io/vscode-cmsis-solution-docs/userinterface.html#cmsis-view) gives you access to the application source code and lets you manage multiple projects, target hardware, and debug configurations.
- The [Run and Debug view](https://mdk-packs.github.io/vscode-cmsis-solution-docs/debug.html#debugger-user-interface) gives you full control over program execution through pyOCD (for ST-Link, CMSIS-DAP and ULink) or J-Link Server.
- The [Trace and Live view](https://mdk-packs.github.io/vscode-cmsis-solution-docs/debug.html#trace-and-live-view) provides real-time variable monitoring while the application runs, and software component viewers for middleware and system services.
- The [Source Control view](https://code.visualstudio.com/docs/sourcecontrol/overview) lets you work directly with Git through a graphical interface. Keil Studio creates the `.gitignore` file for your workspace.

## Get Started

Install this extension and use the [Create New Solution dialog](https://mdk-packs.github.io/vscode-cmsis-solution-docs/create_app.html) in the CMSIS view. Select your board or device to access board-specific examples or blank templates for starting from scratch.

Most [Board Support Packs](https://www.keil.arm.com/boards/) provide a ready-to-run [Blinky example](https://mdk-packs.github.io/vscode-cmsis-solution-docs/create_app.html#examples) for quick verification. By default, the required tools and packs are installed automatically when you build a solution. Optionally, clone projects directly from repositories, such as [github.com/ARM-examples](https://github.com/ARM-examples) using the built-in Git support.

> **Note:** License activation is required for commercial tools but a free [MDK-Community](https://www.keil.arm.com/mdk-community/) license is available for evaluation and non-commercial use. For complete installation instructions, see the [Keil Studio User's Guide](https://mdk-packs.github.io/vscode-cmsis-solution-docs/installation.html).

![CMSIS Solution Quick Tutorial](https://github.com/ARM-software/vscode-cmsis-csolution/raw/main/docs/videos/MDK6_Productivity.gif "CMSIS Solution Quick Tutorial")

## Bare-Metal or RTOS

Keil Studio is designed for all types of embedded projects, ranging from bare-metal firmware to complex RTOS-based systems. It provides direct hardware access, kernel awareness for supported RTOSes, and software component viewers for middleware and system services.

Selecting between [bare-metal](https://arm-software.github.io/CMSIS_6/latest/Core/using_pg.html#using_basic), [Keil RTX](https://www.keil.arm.com/packs/cmsis-rtx-arm), [FreeRTOS](https://www.keil.arm.com/packs/cmsis-freertos-arm), and [Zephyr](https://mdk-packs.github.io/vscode-cmsis-solution-docs/zephyr.html) depends on system complexity, longevity, and non-functional requirements. [Bare-metal](https://arm-software.github.io/CMSIS_6/latest/Core/using_pg.html#using_basic) designs favor simplicity, minimal overhead, and unrestricted hardware control. [FreeRTOS](https://www.keil.arm.com/packs/cmsis-freertos-arm) and [Keil RTX](https://www.keil.arm.com/packs/cmsis-rtx-arm) provide a middle ground, offering multitasking with relatively low overhead. [Zephyr](https://mdk-packs.github.io/vscode-cmsis-solution-docs/zephyr.html) targets product-scale systems that benefit from a rich ecosystem and enforced structure.

## Functional Safety

The [MDK Professional Edition](https://www.keil.arm.com/keil-mdk/#mdk-v6-editions) includes safety features that help developers achieve compliance with standards like ISO 26262 (Automotive), IEC 61508 (Industrial), and IEC 62304 (Medical). It includes the [Arm Compiler for Embedded FuSa](https://developer.arm.com/Tools%20and%20Software/Arm%20Compiler%20for%20Embedded%20FuSa) and the [Arm FuSa Run-Time System](https://developer.arm.com/Tools%20and%20Software/Keil%20MDK/FuSa%20Run-Time%20System). For integration of third-party tools for static code analysis and MISRA checking, Keil Studio creates a standard database.

## Configure Tool Environment

Open a workspace folder and use the [Arm Tools Environment Manager](https://marketplace.visualstudio.com/items?itemName=Arm.environment-manager) to install a compiler, the [CMSIS-Toolbox](https://open-cmsis-pack.github.io/cmsis-toolbox/) with CMake and Ninja, and optionally FVP simulation models. Required [software packs](https://www.keil.arm.com/packs/) for device and board support are installed automatically when creating or building a CMSIS solution, or can be manually added using the `cpackget` command.

## Related

- [Arm Keil Studio for VS Code user's guide](https://mdk-packs.github.io/vscode-cmsis-solution-docs/index.html) explains how to use this IDE.
- [Arm Example projects](https://github.com/Arm-Examples) are complete applications that help you set up your own embedded projects.
- [MDK-Middleware](https://arm-software.github.io/MDK-Middleware/latest/General/working_with_examples.html) provides examples for IPv4 and IPv6 networking, USB Host and Device communication, and File System for data storage.

## Extension Pack

Keil Studio is an extension pack that installs:

- [Arm CMSIS Solution](https://marketplace.visualstudio.com/items?itemName=Arm.cmsis-csolution): Develop embedded applications using CMSIS solutions (csolution projects).
- [Arm CMSIS Debugger](https://marketplace.visualstudio.com/items?itemName=Arm.vscode-cmsis-debugger): Creates the debug platform for embedded applications based on Arm Cortex-M.
- [Arm Tools Environment Manager](https://marketplace.visualstudio.com/items?itemName=Arm.environment-manager):
  Installs development tools specified in a manifest (e.g., Arm Compiler, CMSIS-Toolbox, CMake, Ninja).
- [clangd](https://marketplace.visualstudio.com/items?itemName=llvm-vs-code-extensions.vscode-clangd): Adds intelligent
code features such as completion, diagnostics, and navigation.
- [YAML](https://marketplace.visualstudio.com/items?itemName=redhat.vscode-yaml): Enables syntax support and context help for YAML files.

### Extensions installed with Arm CMSIS Debugger

- [CDT GDB Debug Adapter Extension](https://marketplace.visualstudio.com/items?itemName=eclipse-cdt.cdt-gdb-vscode):
  Debug with gdb or any other debugger that supports the
  [MI protocol](https://sourceware.org/gdb/current/onlinedocs/gdb.html/GDB_002fMI.html).
- [Memory Inspector](https://marketplace.visualstudio.com/items?itemName=eclipse-cdt.memory-inspector): Analyze and
  monitor system memory during development.
- [Peripheral Inspector](https://marketplace.visualstudio.com/items?itemName=eclipse-cdt.peripheral-inspector):
  Displays register-level peripheral information using CMSIS-SVD files.
- [Serial Monitor](https://marketplace.visualstudio.com/items?itemName=ms-vscode.vscode-serial-monitor): View text output from or send text messages to serial or TCP ports.

## Feedback

Submit feedback via our [support page](https://www.keil.arm.com/support/#:~:text=Keil%20Studio%20for%20VS%20Code).

## Telemetry

Keil Studio collects usage data in accordance with
[VS Code telemetry settings](https://code.visualstudio.com/docs/getstarted/telemetry#_disable-telemetry-reporting).
You can adjust telemetry behavior in the VS Code settings menu.

## License agreement

Use of this extension indicates acceptance of the
[End User License Agreement](https://www.keil.arm.com/license-agreement-extensions/).
