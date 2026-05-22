# SpinnyWheels


**SpinnyWheels** is a lightweight procedural caster wheel animation add-on for Blender.  
It automatically rotates and steers caster wheels based on object movement, making it useful for carts, robots, furniture, trolleys, sci-fi vehicles, and other wheeled rigs.
---

## Features

- Automatic caster steering
- Procedural wheel spinning
- Smooth directional interpolation
- Adjustable wheel radius
- Adjustable steering smoothing
- Minimum movement threshold
- Real-time viewport updates

---

## Requirements

- Blender 4.0+

---

## Installation

1. Download the `SpinnyWheel.zip` file
2. Open Blender
3. Go to:

   `Edit → Preferences → Add-ons`

4. Click **Install**
5. Select `SpinnyWheel.zip`
6. Enable **SpinnyWheels - Procedural Caster Animation**

---

## Setup Guide

### Object Structure

Your rig should follow this hierarchy:

```text
Main Object
├── Caster Pivot 1
│   └── Wheel 1
├── Caster Pivot 2
│   └── Wheel 2
```

> **TIP**💡The name of the body or children do not matter. The system works based on hirarchy.

### Important Notes

- The **Main Object** is assigned in the add-on panel
- Each **caster pivot** should rotate on the Z axis
- Each **wheel** should rotate on the X axis
- The add-on automatically detects movement and applies rotation

---

## Using SpinnyWheels

1. Open the **3D Viewport**
2. Open the **Sidebar** (`N` key)
3. Go to the **Casters** tab
4. Enable the system
5. Assign your main object
6. Adjust settings as needed

---

## Settings

| Setting | Description |
|---|---|
| Enabled | Turns the system on/off |
| Main Object | Root object containing caster pivots |
| Wheel Radius | Controls wheel spin speed |
| Smoothing | Controls steering smoothness |
| Min Distance | Minimum movement before updating |

---

## Best Use Cases

- Shopping carts
- Industrial robots
- Warehouse vehicles
- Office chairs
- Sci-fi rovers
- Physics animation helpers

---

## Limitations/Known Bugs

- Addon sometimes freezes when quitting and re-opening Blender. Fix: Go to Edit -> Prefrences -> Addons, Search for SpinnyWheels and disable, then enable again.
- The main object can only have casters as children, any non-caster children will also be treated as casters.
- Multiple rigs cannot be made.

---

## Version

**v0.1**

---

## License

Personal and educational use permitted unless otherwise specified by the author.
