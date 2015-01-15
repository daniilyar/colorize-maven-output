colorize-maven-output
=====================

This repo contains the script for Maven 2-3 output colorizing. The main idea was taken from http://blog.blindgaenger.net/colorize_maven_output.html

The idea is to use sed to insert ansi colors on-the-fly. 
To make Maven output colorized in Linux you can source colorize_maven_output.sh to your .bashrc manually, or just append it to the end of your .bashrc by executing something like this:

   `curl https://raw.githubusercontent.com/daniilyar/colorize-maven-output/master/colorize_maven_output.sh >> ~/.bashrc && . ~/.bashrc`

Please note, that this script is pointing to $MAVEN_HOME variable. If you dont have it in your PATH, you should to add it first. 
Otherwise, if you have M2_HOME variable already, you should update script to point to it instead.

This script preserves mvn`s exit status properly.

Cheet sheet to modify output colors manually:

1. bold = '[1m'
2. blue = '[1;34m'
3. yellow='[0;33m'
4. red = '[1;31m'
5. green = '[1;32m'
6. cyan = '[1;36m'
7. magenta = '[1;35m'
8. black = '[1;30m'
