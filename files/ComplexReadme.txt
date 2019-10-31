UPGRADING THE PROJECT TO LATER VERSIONS OF VISUAL STUDIO SHOULD BE FINE. 
ORIGINALLY INTENDED FOR 2015 BUT TESTED UP TO 2019 AND WORKS FINE.

For building and running the complex application:

1. Confirm the "LuaBindingsDLL" and "Project3D" projects are unloaded (Under the solutions right-click menu).
2. Confirm the "Project2D" project is set to the "StartUp Project" (Under the solutions right-click menu).
3. Set the build settings at the top of Visual Studio to "Debug" and "x86" and build the "Bootstrap", "LuaBindings" and "Project2D" projects.
4. Build/Run the "Project2D" project, it should fail with the following message: "The code execution cannot proceed because lua51.dll was not found. Reinstalling the program may fix this problem.".
5. Close the application and copy "lua51.dll" from the root of the project directory.
6. Navigate to the "AIE-Assignment-ComplexSystem\temp\Project2D\Win32\Debug" directory and paste the "lua51.dll", copied from the previous step.
7. Build/Run the "Project2D" project again. The project should run as planned.


For access to the Demo.lua file (used for coding the example) follow the below steps:

1. Navigate to the projects root directory and open the "bin" folder.
2. Open the Demo.lua file in Visual Studio.