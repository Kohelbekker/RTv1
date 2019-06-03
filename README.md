# RTv1
Simple ray tracing  program

## About RTv1

RTv1 is a simple ray tracing program build on C with SDL2 Library.

Program traces rays from camera to the figures surface and then to the light. Figures can have shading and cast shadows on each other.

Program takes input file, where should be at least one mandatory parameter camera position. Also input file can containe inforamtion about such shapes: sphere, plane, cone, cylinder and light.
Structure of input information:

**Camera**: `[x, y, z]` - start position , `[ox, oy, oz]` rotating angle.

**Sphere**: `[x, y, z]` - shape center , `[R]' - radius, `[r, g, b]` - color, `[L]` - intense of light reflection.

**Cylinder**: `[x, y, z]` - shape center , `[x, y, z]` - central axis, `[r, g, b]` - color, `[R]` - radiusб `[L]` - intense of light reflection.

**Plane**: `[x, y, z]` - shape center , `[x, y, z]` - central axis, `[r, g, b]` - color.

**Cone**: `[x, y, z]` - shape center , `[x, y, z]` - central axis, `[r, g, b]` - color, `[A]` - angle, `[L]` - intense of light reflection.

**Light**: `[x, y, z]` - light center , `[I]` - light intense, `[0 or 1]` - light type (point-light or ambient).

##### Input file example:

<img width="373" alt="7" src="https://user-images.githubusercontent.com/25118092/58816809-f184a680-8632-11e9-84a3-a817ffd04009.png">

SDL2 included from `/framewoks` directory, so you don't need to download additional files.


## Compiling

1. Run `make` after downloading.
2. Run `./RTv1 scenes/[scene_name]`

## Screenshots

<img width="600" alt="1" src="https://user-images.githubusercontent.com/25118092/58816678-a66a9380-8632-11e9-8b69-292cb36f677e.png">

<img width="600" alt="2" src="https://user-images.githubusercontent.com/25118092/58816681-a8345700-8632-11e9-831a-2f50744f79ee.png">

<img width="601" alt="3" src="https://user-images.githubusercontent.com/25118092/58816684-a9fe1a80-8632-11e9-81ec-baf1cf111e67.png">

<img width="598" alt="4" src="https://user-images.githubusercontent.com/25118092/58816687-ab2f4780-8632-11e9-93f1-f24458c33487.png">

<img width="599" alt="5" src="https://user-images.githubusercontent.com/25118092/58816692-acf90b00-8632-11e9-934a-3d6e7404f172.png">
