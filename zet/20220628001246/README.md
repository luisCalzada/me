# apt VS apt-get
apt is intended for humans or interactive use, meaning its interface is a bit more friendly and because of this, it's functions and the way it's used might change in the future,
as long as it's better for humans.
apt-get is not really intended for humans but it's meant to be consistent. So every time it's updated the team makes a hard commit
to make it backwards compatible to keep it consistent.

So what this means is that if **you** human are using the command, you should use apt. But if you are writing a script or if the computer itself will run the command,
you should use apt-get so that even after updates are made to apt-get, the script will run the same.

  #Boost #Linux #CSFundamentals #apt #apt-get #PackageManager 
