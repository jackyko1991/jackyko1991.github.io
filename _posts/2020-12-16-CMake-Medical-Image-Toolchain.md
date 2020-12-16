# CMake Medical Image Toolchain (Qt, VTK, ITK, OpenCV)

To develop desktop medical image software, several essential C++ libraries are recommended for GUI design, graphical rendering and image processing. Here we will provide a detailed instruction on the configuration and compilation of the toolchain.

The toolchain we recommended is cross platform applicable (Windows, MacOS, Linux). The procedure works almost the same on different OS. Also the suggested library packages also provide Python interface for users who are not familiar with C++ coding.

## Dependencies
Beware of software version. Wrong version may cause compilation error.

- [CMake](https://cmake.org/)
- [Qt 5.10.1](https://www.qt.io/)
- [VTK 8.2.0](https://vtk.org/)
- [ITK 4.13.3](https://itk.org/)
- [OpenCV 3.4](https://opencv.org/)

### Associate Python Versions
For users who would like to develop with Python interface, [Anaconda](https://www.anaconda.com/) would include most of the dependent libraries like pyqt and vtk. You may install other necessary packages like OpenCV or ITK via pip or conda.

||C++|Python|
|---|---|---|
|GUI|Qt|pyqt|
|Graphical Rendering|VTK|vtk|
|Image Processing (2D/3D/N-D)|ITK|SimpleITK|
|Image Processing (2D)|OpenCV|OpenCV|

Note that SimpleITK is a lite version of ITK that provides convenient manipulation methods for Python users. ITK also provide Python interface yet is not a popular choice for its relative complex syntax.

## Install Process
We recommend to build the toolchain with following folder hierarchy:

Style 1:
```
.
├── source
│   ├── qt-installer.exe
│   ├── vtk
│   ├── itk
│   └── ...
├── build
│   ├── qt
│   ├── vtk
│   ├── itk
│   └── ...
```

Style 2:
```
.
├── qt
├── vtk
│   ├── build
│   ├── <source-code>
│   └── ...
├── itk
│   ├── build
│   ├── <source-code>
│   └── ...
├── ...
```

### Qt
1. Download [Open Source Qt installer](https://www.qt.io/download-open-source) from official site
2. Follow the install instruction with the correct compiler version.

**Note**: Qt does not provide 64bit MinGW pre-compiled version. 

### VTK
1. Clone the source code 
    ```bash
    git clone -b v8.2.0  https://github.com/Kitware/VTK.git
    ```

### ITK

### OpenCV

## References
- [ITK + VTK + QT on Window 7 64bit and Visual Studio 2010 Pro 32bit project](http://guitarcplusplus.blogspot.com/2013/02/itk-vtk-qt-on-window-7-64bit-and-visual.html)

