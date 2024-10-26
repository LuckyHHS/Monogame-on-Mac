# Monogame-on-Mac

## First Time Install

1. Monogame on mac can be hard. The first step is to install dotnet 6.0.420, and make sure it's the x64 version. Run it and install it.
2. Download VSCode, and add the C# and C# Dev Kit Extensions, also would recommend both monogame extensions.
3. In VsCode open command pallete and select `Install "Code" In PATH`
4. In VsCode terminal run `dotnet new install "MonoGame.Templates.CSharp"`
5. In macos terminal, run `dotnet --version` to check if 6 is installed.
6. Still in the terminal, go to the place where you want to create your project. Run `dotnet new mgdesktopgl -o FOLDERNAME --force`. It if asks to install .net 8.0, do it and install the latest version it is fine.
7. In the macOS terminal, run `dotnet tool install --global dotnet-mgcb --version 3.8.1.303`, do this for `dotnet-mgcb-editor`, `dotnet-mgcb-mac`, `dotnet-mgcb-linux`, and `dotnet-mgcb-windows`. **MAKE SURE YOU DOWNLOAD VERSION 3.8.1.303**. Restart VSCODE. Follow the New Projects Down below.

## New Projects

1. Run in terminal "dotnet new mgdesktopgl -o FOLDERNAME --force" if you havent created your project already.
2. Open it in VSCode and in the .csproj change the package reference to `3.8.1.303`, and target framework at the top to net6.0. Then go to .config then into `dotnet-tools.json`. Change all the versions to `3.8.1.303`. In the VSCode terminal run `dotnet tool restore`. Make sure in the terminal output it says stuff about loading version `3.8.1.303`.
3. Make sure you build it once before opening content manager. It should work now.

