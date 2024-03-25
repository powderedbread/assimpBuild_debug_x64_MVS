
***This is only for "debug" 64 bit windows visual studio 2022 at the moment.



1. Make sure you have a .cpp file in your project to access c++ properties.
2. Right click your solution and go to properties.  Make sure you have x64 and "debug" selected in the top boxes.

3. Go to C/c++ > general
Click on Additional Include Directories
Type the path where you copied the include folder to.  The final path should end in \indlude because when you type "#include" at the top of your file it will look like #include <assimp/scene.h>>

4. Then go to "Linker" > General
And type in the path to the lib folder.  The path should end in \lib

5. Then go to Linker > Input
and add "assimp-vc143-mtd.lib"

That should be about it.  Make sure you have x64 and debug selected on top when you try to run the program as well.
***note, I dont know if you need the dll in the lib folder, but one in the root folder is the same dll.  Its there for convenience since you need to copy and paste it.
.
