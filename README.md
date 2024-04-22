# JUCE install and update script for cmake

After running this script in the console, JUCE is installed (or updated in case of a new JUCE version) globally on your Mac in the /opt/local/libexec folder.
Then you can access JUCE in CMakeLists.txt with

    find_package (JUCE CONFIG REQUIRED PATHS "/opt/local/libexec")

to use it in your C++ app. As a prerequisite, git and cmake must be installed.
Place this script under

    /opt/local/bin/juce_install (without file extension)

and make it executable with

    sudo chmod +x /opt/local/bin/juce_install

so you can use it from anywhere with the console command

    juce_install


> __Be aware: This script was created quickly without much testing. There is no guarantee and you should know what you are doing and use the script on your own responsibility and risk!__
