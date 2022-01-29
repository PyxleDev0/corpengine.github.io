
# CORP Engine Colors

| Table of Contents | 
| ----------- |
| [1.1 - List of Colors](#colors-list) |
| [1.2 - Color Functions](#color-functions) |



* Colors in CORP are constants in the `main.Colors` module, thus you can access each color with `corpengine1.Colors.{COLOR}.`
* Each color is defined as a **tuple** following the pattern `(RED, GREEN, BLUE)`, having a length of **3**, each item being an integer between 0 and 255 (both inclusive) representing the intesity of the corresponding color.

<span id="colors-list"></span>
## 1.1 - List of Colors
### Black - White Tones
        WHITE
        CORPWHITE
        LIGHTGRAY
        SILVER
        GRAY
        DARKGRAY
        BLACK
### Single Colors (Single Tone)
        RED
        LIME
        BLUE

### Single Colors (Toned)
        DARKGREEN
        DARKRED
        GREEN

### Double Colors (Single Tone)
        MAGENTA
        AQUA
        YELLOW

### Double Colors (Toned)
        LIGHTBLUE
        ORANGE

### Triple Colors (Toned)
        PINK
        VIOLET
        BROWN
        TAN
        FORESTGREEN
        BABYBLUE

<span id="color-functions"></span>
## 1.2 - Color Functions
There are a few useful functions in CORP that let you work with tuples representing colors. The current functions are `mix`,`onlyEmpty`,`onlyFill` and `all`.
See usage below.
### 1.2.1 - Mix
### 1.2.1 - Only Empty
### 1.2.1 - Only Fill
### 1.2.1 - All

---
Written January 29, 2022 by LercDsgn
