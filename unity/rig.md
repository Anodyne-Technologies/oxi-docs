---
layout: default
title: OXI Rig
parent: Unity
nav_order: 2
---

## What it does
Centralizes wiring of providers to head/hand targets with optional origin offset.

## Fields
- `head`, `leftHand`, `rightHand`
- `hmdPose`, `leftPose`, `rightPose`
- `origin`
- `applyOriginOffset`

## Origin composition
`PoseWithOriginUtility.Compose(origin, local)` aligns the rig to a play area.

## Minimal scene graph
Can live on one GameObject. Receivers are added automatically if missing.
