---
layout: default
title: Pose Pipeline (Input System)
parent: Unity
nav_order: 1
---

## Provider
`InputActionPoseProvider` reads a single Pose action (preferred) or position+rotation actions. Actions auto-enable/disable and publish `Pose` on performed.

## Receiver
`PoseReceiver` applies poses to a `Transform` in World or Local space.

## Inspector
Assign `InputActionReference`s for HMD and hands. Actions should be **Pass Through** with control type **Pose**.

## Bindings
- HMD: `<XRHMD>/centerEyePose`
- Left hand: `<XRController>{LeftHand}/devicePose`
- Right hand: `<XRController>{RightHand}/devicePose`

## Troubleshooting
- No value? Ensure actions are Pass Through and device is plugged in.
- Input System must be active in Project Settings.
