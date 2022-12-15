# LinuxCmds

# check given port(portNo) is used by which process 
sudo lsof -i -P -n | grep portNo

# check given process(pid) use which all ports
sudo lsof -aPi -p PID

# check file is used by which process
sudo lsof /var/lib/dpkg/lock-frontend

**#locate installed package files**

$dpkg -L <package-name>  
for eg.
$dpkg -L libsdl2-2.0-0

**change ubuntu resolution**
  
cvt 1600 900
  
xrandr --newmode "1600x900_60.00"  118.25  1600 1696 1856 2112  900 903 908 934 -hsync +vsync

xrandr --addmode eDP-1 1600x900_60.00

**// go to previous dir**
  
$ cd - 

**  //this is stack **
  
$ pushd /var
/var /etc   

$ popd  // will take you to /etc

**send process to backgound**
  
$ ctrl + z // send process to baclgound
  
$ fg // bring process to foregroud


$ sudo !!  // run previous cmd with sudo


**History Cmds**

$ history  //show list of previous cmds ran on system

$ HISTTIMEFORMAT='%d/%m/%y %T'  // variable to print the history with time and date

HISTTIMEFORMAT='%d/%m/%y %T' 
  
HISTSIZE = 1000                       // history file size
  
HISTFILE = ~/.bash_history            // history file name
  
HISTIGNORE = "ls*"
  
HISTIGNORE = "[ \t]*"
  
add "[ \t]*" to your HISTIGNORE variable you can make any command be ignored by starting it with a space.


102  cd -
  
103  pwd
  
104  cd /var
  xrandr --newmode "1600x900_60.00" 118.25 1600 1696 1856 2112 900 903 908 934 -hsync +vsync xrandr --addmode eDP-1 1600x900_60.00
105  fg

$ !102  //this will execute the cmd from history at index 102

$fc -e: 102 105

fc is used to list or edit and re-execute commands from the history list.
    FIRST and LAST can be numbers specifying the range, or FIRST can be a
    string, which means the most recent command beginning with that
    string.
    
    Options:
      -e ENAME	select which editor to use.  Default is FCEDIT, then EDITOR,
    		then vi
      -l 	list lines instead of editing
      -n	omit line numbers when listing
      -r	reverse the order of the lines (newest listed first)


**// will print matrix movie screen //just for fun**
  
$ cmatrix 


**// will list live updates to file**
  
$ tail -f <filename>    

**//will empty the file**
  
$ truncate -s -o <filename>    


