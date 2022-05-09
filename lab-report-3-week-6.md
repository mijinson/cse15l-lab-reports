# Working on ieng6 Server

## Streamlining ssh Configuration
### Log into the ieng6 server using an alias username and no password

Steps:

1) make sure ssh keys are set up refer to lab report 1 Remote Access Tutorial under setting SSH Keys section.

2) Log into the ieng6 server using `ssh cs15lsp22zzz@ieng6.ucsd.edu` then use `cd .ssh` to go to the correct directory where the ssk keys are stored and where the config file will be stored. Add a file config in the directory using `touch config`. The image below uses the command `ls` to confirm all files are present in the .ssh directory.

![image](lspic.png)

IMPORTANT NOTE: to find the files created in the .ssh make sure to look in the correct path locations.
example: Users/username/.ssh/config.

3) In the config file add the following lines of code shown in image.

![image](configimage.png)

4) Next to Host the ieng6 can be replaced with any alias. For instance ucsd. Now type in terminal `ssh alias` alias is either ieng6 or can be changed to any name replaced after Host.

The `scp` command can now also work using the alias name instead of the long course specific username.

refer to image below

![image](scpimage.png)