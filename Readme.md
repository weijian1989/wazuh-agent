# General Build Script
## Index
- [General Build Script](#general-build-script)
  - [Index](#index)
  - [Purpose](#purpose)
  - [Dependencies](#dependencies)
  - [Compile Wazuh](#compile-wazuh)
  - [How to use the tool](#how-to-use-the-tool)
    - [Optional arguments:](#optional-arguments)

## Purpose
The `build.py` script was created to compile, test and validate the available modules and its code readiness. This tool was meant to developers to speed up the code readiness checking and development and to be able to include the usage of the tool as part of automation processes and checks.

## Dependencies
There are several modules needed in order to the tool to work correctly.
  - cppcheck
  - valgrind
  - lcov
  - gcov
  - astyle
  - scan-build-12

## Compile Wazuh
In order to run unit tests on a specific wazuh target, the project needs to be built with the `DEBUG` and `TEST` options as shown below:
```
make TARGET=agent DEBUG=1  wazuh-agent
```

