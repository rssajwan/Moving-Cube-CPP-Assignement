# Moving Cube in C++

A simple C++ project that renders a rotating 3D cube in the terminal using ASCII characters. The project demonstrates the fundamentals of 3D graphics without relying on any external graphics libraries.

## Features

- 3D rotating ASCII cube
- Perspective projection
- Z-buffer for hidden surface removal
- Real-time terminal rendering
- Built entirely with standard C++

## Concepts Used

- 3D coordinate transformations
- Rotation using sine and cosine
- Perspective projection
- Depth buffering (Z-buffer)
- Rendering loop
- ANSI escape sequences for terminal output

## Build and Run

Compile with g++:

```bash
g++ main.cpp -o cube
```

Run:

```bash
./cube
```

On Windows:

```bash
cube.exe
```

## Project Structure

```
Moving-Cube-CPP/
├── main.cpp
└── README.md
```

## Purpose

This project was created as a learning exercise to better understand the mathematics behind 3D rendering and to practice implementing graphics algorithms in C++ without using OpenGL or other graphics libraries.
