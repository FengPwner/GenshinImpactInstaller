# Genshin Impact Cross-Platform Auto-Installer


## Introduction

This is an automated installation tool based on Shell and Python, designed to help players download and install Genshin Impact with a single click. The script supports cross-platform execution, automatically detecting the current operating system and processor architecture to download the corresponding official installation package.


## Core Features

Cross-Platform Support: Perfectly compatible with Windows (Git Bash/WSL) and Android (Termux) environments.

Smart Architecture Detection: Automatically detects device processor architecture (x86_64 or ARM64) to download matching packages.

Dynamic Script Generation: In Windows environments, it automatically builds and invokes a  .bat  script to execute download tasks.

Auto-Trigger Installation: After downloading, it automatically triggers the system installation interface on Android devices and opens the launcher installer on Windows.

Fallback for Unknown OS: When running on unsupported systems, it waits for 5 seconds and then automatically redirects to the official Genshin Impact website.

Native Python Validator: Includes a URL validation script written in pure native libraries, requiring no third-party dependencies to check link validity.


## File Structure

 Install_NoCN.sh : Main installation script, responsible for environment detection, downloading, and triggering installation.

 test_NoCN.py : Link validation tool, used to check if official APIs are valid before installation.

 README.md : Project documentation.


## Quick Start


1. Validate Download Links (Optional)

Before running the installation script, it is recommended to verify if the official links are available: