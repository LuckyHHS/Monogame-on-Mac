# Monogame-on-Mac

## First Time Install

1. Monogame on mac can be hard. The first step is to install dotnet 6.0.420, and make sure it's the x64 version. Run it and install it.
2. Download VSCode, and add the C# and C# Dev Kit Extensions, also would recommend both monogame extensions.
3. In VsCode open command pallete and select Install "Code" In PATH
4. In VsCode terminal run "dotnet new install "MonoGame.Templates.CSharp""
5. In macos terminal, run dotnet --version to check if 6 is installed.
6. Still in the terminal, run "dotnet new mgdesktopgl -o FOLDERNAME --force". It if asks to install .net 8.0, do it and install the latest version it is fine.
7. 12. Open the csproj file and find package refrence and change the version to 3.8.1.303,  and target framework at the top to net6.0.
8. Uninstall all dotnet mgcb editors by running in the vs code terminal, "dotnet tool uninstall dotnet-mgcb-editor". Do this this mgcb-linux, windows, and mac, and also just do "dotnet-mgcb". It should be 5 different ones.
9. Install the version 3.8.1.303 by doing "dotnet tool install dotnet-mgcb-editor-windows --version 3.8.1.303", and make sure you do this for mac, linux, and also just "dotnet-mgcb-editor" and "dotnet-mgcb". This should be 5 new ones.
10. Run "dotnet restore"
11. Run "dotnet tool restore"
12. Build using C# and make sure you build it once before opening the content manger.



## New Projects

1. Run in terminal "dotnet new mgdesktopgl -o FOLDERNAME --force"
2. Open it in VSCode and in the .csproj change the package reference to 3.8.1.303, and target framework at the top to net6.0.
3. Make sure your restore tools and build it once before opening content manager.

