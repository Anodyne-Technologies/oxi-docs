---
layout: default
title: Installation
parent: Getting Started
nav_order: 1
---

## Requirements
- Unity 6
- `com.unity.inputsystem` (verified version)
- Windows or Mac

## Install OXI
1. Add the package via Git URL or local path.
2. Ensure your asmdef references `Unity.InputSystem`.

## Enable Input System
Project Settings → Player → Active Input Handling = **Input System** (or Both).

## Package Manifest
```json
{
  "dependencies": {
    "com.unity.inputsystem": "1.10.0"
  }
}
```

## Verify
Compile succeeds with no missing references.
