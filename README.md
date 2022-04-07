
# Black & Scholes PDE simulation (w/ 1D diffusion equation transformation)

## Introduction

This current project has multiple objectives : 
- study theory behind Black-Scholes formula, Ito lemma and its PDE representation
- study finite difference methods and its differents domain discretization models involving implicit and theta-schema stencils
- transform the main PDE into a so-called "Reduced PDE" representing 1D-diffusion equation
- create and implement an optimized oriented-object structure
- develop a complete and enhanced wrapper of the SDL2 library (sdl2 + sdl2_ttf) to handle graphic/text configuration with much more flexibility

## Set up & Execution

### Dependencies

In order to plot the solutions and the numerical error between the two implemented methods, we are using **SDL2** library (Simple DirectMedia Layer).

According to the host machine, follow the instructions on [this page](https://wiki.libsdl.org/Installation).

### Setting up step-by-step

```bash
git clone https://github.com/lcsrodriguez/ENSIIE_S3_PAP_BLACK_SCHOLES_CPP.git
cd ENSIIE_S3_PAP_BLACK_SCHOLES_CPP
```

To generate a full and well-styled technical documentation of the project, please type :
```bash
doxygen Doxyfile
```

To execute the main program, please execute the following block :
```bash
cd source
rm projet
g++ -g -Wall -Wextra -o projet *.cpp `pkg-config --cflags --libs sdl2 sdl2_ttf`
./projet
```

**Important remark** : The `sdl2_ttf` has been added to the `pkg-config` of the block above to handle text printing configuration. It's the only external dependency of this project.

## License & Copyrights

**Lucas RODRIGUEZ** (2021 - 2022)

Academic works released during December 2021 & January 2022