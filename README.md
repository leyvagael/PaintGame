# 🎨 Paint

A Python implementation of a simple drawing application, built using the `turtle` graphics library and the `freegames` package. By Gael Leyva and Emma Sofía García.

## Overview

The player can draw various shapes on a blank canvas by clicking two points on the screen — the first click sets the starting point and the second draws the selected shape. Colors and shapes can be switched at any time using keyboard shortcuts, and any stroke can be undone.

## Requirements

- Python 3.x
- [`freegames`](https://pypi.org/project/freegames/) library

Use a virtual environment to create an isolated workspace for a project’s dependencies and Python version.
This prevents package conflicts between projects and keeps your system installation clean.

```bash
sudo apt -get install python3-all-venv
python3 -m venv ./games/
source ./games/bin/activate
```

Install the dependency with:

```bash
python3 -m pip install freegames
```

## How to Run

```bash
python3 paint.py
```

## Controls

### Shapes

| Key | Shape |
|---|---|
| `l` | Line |
| `s` | Square |
| `c` | Circle |
| `r` | Rectangle |
| `t` | Triangle |

### Colors

| Key | Color |
|---|---|
| `K` | Black |
| `W` | White |
| `R` | Red |
| `G` | Green |
| `B` | Blue |
| `P` | Pink |

### Other

| Key | Action |
|---|---|
| `u` | Undo last stroke |

## Changes from the Original

### 1. Extra color
Pink was added as an additional color option, accessible with the `P` key.

### 2. Circle
A circle drawing function was implemented. The radius is determined by the horizontal distance between the two clicked points.

### 3. Rectangle
A rectangle drawing function was implemented. The width and height are each determined independently by the horizontal and vertical distance between the two clicked points.

### 4. Triangle
An equilateral triangle drawing function was implemented. The side length is determined by the horizontal distance between the two clicked points.
