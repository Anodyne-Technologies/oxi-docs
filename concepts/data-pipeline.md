---
layout: default
title: Data Pipeline (Providers & Receivers)
parent: Concepts
nav_order: 1
---

## Contracts
- `IDataProvider<T>`: `IsValid`, `Timestamp`, `TryGetValue(out T)`, `event OnValueChanged`.
- `IDataReceiver<T>`: `SetProvider(IDataProvider<T>?)`.

## Unity Base Classes
- `BaseDataProvider<T>`: `RaiseValueChanged(T)`, timestamps via `Time.realtimeSinceStartupAsDouble`.
- `BaseDataReceiver<T>`: safe subscribe/unsubscribe on enable/disable; inspector provider slot; pulls initial value on set.

## Usage
```csharp
class FloatProvider : BaseDataProvider<float>
{
    public void Push(float v) => RaiseValueChanged(v);
}

class FloatReceiver : BaseDataReceiver<float>
{
    protected override void OnValueChanged(float v)
    {
        // apply value
    }
}
```
