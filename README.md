# Moving Cube in C++ (ASCII Graphics)

A terminal-based graphics project that renders a rotating 3D cube using only ASCII characters and mathematical transformations. This project is a C++ recreation of the famous ASCII spinning cube demonstration, built from scratch to better understand the mathematics behind 3D graphics, projection, and terminal rendering.

---

## 📖 About

This project demonstrates how a three-dimensional cube can be represented and animated entirely inside a terminal window without using any graphics libraries such as OpenGL, DirectX, or SDL.

Instead of drawing pixels, the program continuously calculates the positions of points on each face of a cube, projects those 3D coordinates onto a 2D terminal screen, and renders them using ASCII characters. The result is a rotating cube displayed directly in the console.

The primary goal of this project was to gain a deeper understanding of:

- 3D coordinate systems
- Rotation matrices
- Perspective projection
- Z-buffering (Depth Buffer)
- Real-time rendering loops
- Terminal graphics using ANSI escape sequences
- Implementing mathematical concepts in modern C++

---

## ✨ Features

- Rotating 3D ASCII cube
- Perspective projection from 3D to 2D
- Hidden surface removal using a Z-buffer
- Real-time terminal rendering
- Pure C++ implementation
- No external graphics libraries required
- Cross-platform logic (uses standard C++ with ANSI-compatible terminals)

---

## 🛠 Technologies Used

- C++
- Standard Template Library (STL)
- `<cmath>`
- `<cstring>`
- `<chrono>`
- `<thread>`
- ANSI Escape Sequences

---

## 📚 Concepts Learned

This project helped reinforce several important computer graphics concepts:

### 3D Rotation

Each point of the cube is rotated around different axes using trigonometric functions.

```cpp
sin()
cos()
```

The program computes new coordinates after every frame to create continuous rotation.

---

### Perspective Projection

After rotating the cube, every 3D point is projected onto a 2D terminal screen.

The projection gives the illusion of depth by making distant points appear smaller than nearby ones.

---

### Z-Buffer

A depth buffer stores the closest point drawn for every screen position.

This prevents faces hidden behind other faces from being rendered over the front ones.

---

### Rendering Loop

The animation works by repeatedly performing these steps:

1. Clear the screen buffer.
2. Clear the depth buffer.
3. Rotate cube points.
4. Project points onto the screen.
5. Update the terminal.
6. Repeat.

---

## 📂 Project Structure

```
Moving-Cube-CPP/
│
├── main.cpp
├── README.md
```

---

## 🚀 Building the Project

Compile using g++:

```bash
g++ main.cpp -o cube
```

Run:

```bash
./cube
```

Windows:

```bash
cube.exe
```

---

## 📸 Output

The program continuously renders a rotating ASCII cube directly inside the terminal.

Example output:

```
       #######
     ###$$$$$$
    ##$$$$$$$$
   ##$$$$$$$$$
    ##$$$$$$$
      #######
```

(The actual animation is continuous.)

---

## 🧠 Challenges Faced

During development several problems were encountered, including:

- Understanding perspective projection
- Implementing rotation using trigonometric functions
- Correctly indexing the screen buffer
- Debugging the depth (Z) buffer
- Clearing and updating the terminal efficiently
- Translating C code into modern C++ while preserving functionality

Working through these challenges significantly improved my understanding of both C++ and introductory computer graphics.

---

## 🎯 Learning Outcomes

After completing this project, I gained practical experience with:

- Mathematical programming
- Geometry in computer graphics
- Memory management using arrays
- Real-time rendering loops
- Debugging graphical algorithms
- Converting procedural C programs into modern C++

---

## 🔮 Future Improvements

Possible future enhancements include:

- Adjustable cube size
- Keyboard controls
- Multiple cubes
- Colored ASCII rendering
- Lighting and shading
- Different rotation speeds
- FPS counter
- Object-oriented refactoring
- OpenGL implementation for comparison

---

## 🙏 Acknowledgements

This project was inspired by the well-known **ASCII Spinning Cube** demonstration and was recreated in C++ as a learning exercise to better understand how 3D rendering works under the hood.

---

## 📄 License

This project is intended for educational purposes and personal learning.

Feel free to fork, modify, and experiment with the code.

---

## 👨‍💻 Author

**Rishabh Sajwan**

Learning C++ through hands-on projects and exploring computer graphics from first principles.
