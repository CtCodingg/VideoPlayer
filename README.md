# VideoPlayer
VideoPlayer based on Qt and GStreamer

# Installation
## Linux
	1. Navigate into repo
	2. "mkdir build && cd build"
	3. "cmake .."
	4. "cmake --build . --config Debug"

## Windows
	1. Use cmake to generate project, build for example with visual studio
	2. Navigate into the qt installation folder to the windeployment tool (e.g. "C:\Qt\6.9.0\msvc2022_64\bin")
	3. windeployqt.exe --qmldir <path-to-app-qml-files> <path-to-app-binary>
	
