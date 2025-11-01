# AUTOSAR Development Projects

This repository section focuses on AUTOSAR (AUTomotive Open System ARchitecture) implementations and projects.

## Structure

### 1. COM_Stack
Communication stack implementations and configurations for AUTOSAR-based systems.

### 2. Projects
#### AUTOSAR Door Lock Project
A comprehensive automotive door lock system implementation featuring:
- **ARXML Configurations**
  - Base AUTOSAR schema (AUTOSAR_00046.xsd)
  - ECU Configuration Parameters
  - Platform Types definitions
- **Development Workspace**
  - Door Lock Indication module
  - RTE Generator configuration
- **Code Implementation**
  ```
  - OS-based implementation
  - Build scripts (Python and Batch)
  - STM32F107 target support
  ```

### 3. Software_Layers
Contains modular AUTOSAR software implementations:

#### a. Interface Configurations (Lab2)
- AUTOSAR interface definitions
- Platform type configurations
- Base AUTOSAR schema implementation

#### b. Software Component Configurations (Lab1)
- Basic software component setups
- Platform types definitions
- ARXML configurations

#### c. Door Lock Project Implementation
- Complete software layer architecture
- HAL implementations
- STM32F103C6 driver support
- CMSIS V5 integration

## Technical Stack

- **Target Hardware**: STM32F103C6, STM32F107
- **Development Tools**:
  - AUTOSAR Builder
  - RTE Generator
  - ARXML Configuration Tools

## Project Setup

1. **Environment Setup**
```batch
@echo off
set PATH=<your-toolchain-path>;%PATH%
```

2. **Building the Project**
```batch
// For building:
learnInDepth_build.bat

// For cleaning:
learnInDepth_clean.bat
```

## AUTOSAR Configuration

The project uses standard AUTOSAR 4.x configurations with:
- Software Components (SWC)
- Runtime Environment (RTE)
- Basic Software (BSW)
- ECU Configuration

## Key Files

- `AUTOSAR_Packages_Configuration.arxml`: Main AUTOSAR configuration
- `PlatformTypes.arxml`: Platform-specific type definitions
- `Software_Component.arxml`: SWC configurations
- `Interfaces.arxml`: Interface definitions

## Development Guidelines

1. Always validate ARXML files against schema
2. Follow AUTOSAR naming conventions
3. Use provided build scripts for consistency
4. Maintain proper layering according to AUTOSAR architecture

## Requirements

- AUTOSAR Builder/Designer tool
- STM32 development environment
- ARM compilation toolchain
- Python 3.x (for build scripts)

Note: Specific version requirements and additional setup instructions should be added based on your project's needs.
