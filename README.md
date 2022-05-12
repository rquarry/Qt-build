# Building Qt 5 on Windows 10

Using this [Qt doc as a guide](https://wiki.qt.io/Building_Qt_5_from_Git#Getting_the_source_code) use these specifics:

1. Install visual studio 2022 (to-do: Find more details of needed install config)
2. Install [chocolatey](https://chocolatey.org/install) for easy windows package management
3. run ```choco install git python perl choco install strawberryperl``` to install build deps
4. Use the ``` qt5vars.bat``` in this repo
5. Clone the Qt repo and checkout the most recent ```LTS/release``` branch per [this page](https://wiki.qt.io/Branches) (5.12.6 as of this commit).
6. Run the perl command prompt, switch to the qt directory and run ``` perl --module-subset=qtbase``` to just build the base qt libs
7. Follow the direction to make a shadown build dir, configure, and make
