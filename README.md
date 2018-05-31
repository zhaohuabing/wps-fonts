Original article: https://askubuntu.com/questions/861588/wps-office-equation-editor

For the first issue you need a set of fonts for WPS and this should be dropped into the /usr/share/fonts folder for system wide access.

Now I have created a git repo with these fonts download it from here and add it like this:

download fonts from here
create a folder sudo mkdir /usr/share/fonts/kingsoft
copy the contents of that download to folder in (2)
run sudo chown -R $USER:$USER /usr/share/fonts/kingsoft
run sudo chmod -R o+rw,g+rw /usr/share/fonts/kingsoft or leave as is if it has read and write permissions for owner (you)
run sudo fc-cache -vfs
For the second issue. You could try this qalculate:

Install: sudo apt-get install qalculate

Qalculator resource: https://www.maketecheasier.com/qalculate-powerful-calculator-for-linux/
