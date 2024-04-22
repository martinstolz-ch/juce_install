# JUCE install / update script for cmake

## Purpose

After running the __juce_install__ script in a console window, JUCE is installed (or updated in case of a new JUCE version) globally on your Mac in the __/opt/local/libexec__ folder.
Then you can access JUCE in CMakeLists.txt with 

<code>find_package (JUCE CONFIG REQUIRED PATHS "/opt/local/libexec")</code>

to use it in your C++ app. 

The target path __/opt/local/libexec__ can be changed from within the script by changing the variable __juce_install_dir__

## Install the script

1. Make sure that __git__ and __cmake__ are installed on your Mac.
2. Open a console window and change to the directory where you want the script to be installed.
3. Clone THIS repository

<code>git clone https://github.com/martinstolz-ch/juce_install_script.git</code>

4. Change to the juce_install_script directory

<code>cd juce_install_script</code>

5. Make the script executable

<code>sudo chmod +x juce_install</code>

6. Run the script in the console

<code>juce_install</code>


> __Be aware: This script was created quickly without much testing. There is no guarantee and you should know what you are doing and use the script on your own responsibility and risk!__
