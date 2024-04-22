# JUCE install script for cmake

After running this script in the console, JUCE is installed globally on your Mac in the /opt/local/libexec folder.
Then you can find JUCE in CMakeLists.txt with

    find_package (JUCE CONFIG REQUIRED PATHS "/opt/local/libexec")

to use it in your C++ app. 
As a prerequisite, git and cmake must be installed.
Place this script under

    /opt/local/bin/juce_install (without file extension)

and make it accessible with

    sudo chmod +x /opt/local/bin/juce_install

directly in the console.
