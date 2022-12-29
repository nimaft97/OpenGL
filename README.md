# OpenGL

## SETUP
The combination that I prefer to use is Visual Studio and Windows. However, I used GLFW to create a box that is compatible with all three major OSs
- Download GLFW binaries from [here](https://www.glfw.org/download.html)
- Copy the `include` folder and the latest `lib` folder to dependencies folder
- Link them to the project in Visual Studio (e.g., properties -> C/C++ and linker). For better robustness, use relative directories instead of abolute paths
- Download GLEW binaries from [here](https://glew.sourceforge.net/)
- Copy `include` and `lib` folder to dependencies folder (I linked static libraries instead of dll)
- Link them to the project in visual studio
- If GLEW's static lib is linked, go to properties -> C/C++ -> preprocessor and add `GLEW_STATIC` to the preprocessor definitions


## Run
- Use the main file from [here](https://www.glfw.org/documentation.html)
- In order to use GLEW, make sure to import glew before other OpenGL-related libraries
- First you need to create a valid OpenGL rendering context (e.g., `glfwMakeContextCurrent(window);`) and then call glewInit() to initialize the extension entry points
