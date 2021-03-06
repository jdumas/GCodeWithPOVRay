# GCodeWithPOVRay
A tool for fancy visualization of 3D printing GCdoes with [POV-Ray](http://www.povray.org/download/).

## Main idea
Provided an input 3D printing GCdoe file by the user, this tool generates a POV-Ray rendering file containing smooth geometries imitating the pushing filament along the printing paths in the GCdoe. Then the user will be able to render the prints by loading the rendering file with [POV-Ray](http://www.povray.org/download/).

An example is illustrated below, which is the rendered print of a "kitten" model slicing with [IceSL](http://shapeforge.loria.fr/icesl/):
![](/example/kitten.png)

This tool has been used in several research projects, such as:
* [Anti-aliasing for fused filament deposition](https://arxiv.org/abs/1609.03032)
* [Colored fused filament fabrication](https://arxiv.org/abs/1709.09689)

## Contributors
* [Haichuan Song](https://github.com/shcig) (haichuansong@gmail.com)
* [Sylvain Lefebvre](http://www.antexel.com/sylefeb/research)

## Dependency
For rendering, the user need to install [POV-Ray](http://www.povray.org/download/). For more information about the rending parameters and how to render on POV-Ray, please refer to the offical site of POV-Ray.

## Compile
The project is developed in C++, and there is only one source file. A cmake CMakeLists.txt is provided, with which should be easy to generate projects for desired developing tools. This project compiles well with Visual Studio 2013 and later versions, though have not been tested much on other platforms.

## How to use
After compling, the user can run the executable file aided with a "configurations.txt" file in the same folder to generate the rendering file. For more details, please refer to the "example" folder.

Have fun with it, questions and suggestions are also welcome!
