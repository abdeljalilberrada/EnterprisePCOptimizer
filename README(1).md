# Enterprise PC Optimizer Pro

Professional Windows optimization, diagnostics, repair, and maintenance
utility designed for enterprise and administrative workstations.

**Developer:** Abdeljalil Berrada\
**Platform:** Windows 10 / Windows 11\
**Edition:** Enterprise

------------------------------------------------------------------------

## Overview

Enterprise PC Optimizer Pro helps technicians diagnose, maintain,
repair, and optimize Windows workstations through a professional
interface.

The project focuses especially on common issues found on administrative
and enterprise PCs, including high disk usage, temporary file
accumulation, Windows health, storage maintenance, system integrity,
network maintenance, and performance diagnostics.

The application performs safety and diagnostic checks before heavier
maintenance operations whenever appropriate.

------------------------------------------------------------------------

## Main Features

-   Smart PC diagnostics
-   Disk 100% analysis
-   CPU, RAM, storage, SSD and HDD information
-   Windows health checks
-   Temporary file and cache cleanup
-   SSD TRIM and HDD optimization
-   Windows component maintenance
-   DISM and SFC integration
-   Windows Update maintenance
-   Microsoft Defender maintenance
-   Network maintenance
-   Restore point support
-   Technician reports
-   Application diagnostics
-   Backup and restore
-   GitHub synchronization
-   Automatic updates through GitHub Releases
-   Optional remote configuration for enterprise deployments
-   Workstation identification
-   Maintenance / emergency control support
-   Keyboard shortcuts and fullscreen mode

------------------------------------------------------------------------

## Safety

The application can check relevant system conditions before maintenance,
including administrator privileges, disk state, free space, pending
reboot state, and existing Windows maintenance processes.

A Windows System Restore Point can be created before important
optimization operations.

> Always validate a new release on a test workstation before deploying
> it across enterprise PCs.

------------------------------------------------------------------------

## Automatic Updates

Enterprise PC Optimizer Pro supports automatic updates through GitHub.

The application reads `version.json` from this repository. When a newer
version is published, the updater can download the official
`EnterprisePCOptimizer.exe` asset from GitHub Releases and offer
installation.

The README does **not** need to be edited for every application update.
Version-specific information belongs in `version.json` and the
corresponding GitHub Release.

------------------------------------------------------------------------

## Remote Configuration

Enterprise deployments can optionally use `remote_config.json` for
centralized application controls such as:

-   Global maintenance mode
-   Emergency lock
-   Global information messages
-   Minimum supported application version
-   Forced update requirements
-   Workstation-specific rules

The application remains designed to operate locally when Internet
connectivity is unavailable.

------------------------------------------------------------------------

## Installation

1.  Open the **Releases** section of this repository.
2.  Download `EnterprisePCOptimizer.exe` from the latest release.
3.  Run the application on Windows.
4.  Approve the Administrator/UAC prompt when system-level maintenance
    is required.

The compiled executable does not require a separate Python installation.

------------------------------------------------------------------------

## Supported Systems

-   Windows 10 64-bit
-   Windows 11 64-bit

Some maintenance operations require Administrator privileges.

------------------------------------------------------------------------

## Repository Structure

``` text
EnterprisePCOptimizer/
├── README.md
├── version.json
└── remote_config.json

GitHub Releases
└── EnterprisePCOptimizer.exe
```

`README.md` is the permanent project description.

`version.json` is updated when a new application version is released.

`remote_config.json` is changed only when remote enterprise behavior
needs to be modified.

The executable itself is distributed through **GitHub Releases**, rather
than committing each executable build to the repository.

------------------------------------------------------------------------

## Release Workflow

For each new application version:

1.  Build `EnterprisePCOptimizer.exe`.
2.  Create a new GitHub Release with the matching version tag.
3.  Upload `EnterprisePCOptimizer.exe` as the Release asset.
4.  Update `version.json`.
5.  Update `remote_config.json` only if necessary.

**You do not need to rewrite this README for every release.**

------------------------------------------------------------------------

## Developer

**Abdeljalil Berrada**

Enterprise PC Optimizer Pro
