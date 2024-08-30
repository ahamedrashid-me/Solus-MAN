
HOW TO INSTALL ANY .deb (DEBIAN/UBUNTU) PACKAGE TO eopkg(SOLUS LINUX) ???


#step by step:--

1/ Open your terminal(ctrl+shift+t) in linux system(in solus linux)

2/ type those command in your terminal:

	sudo eopkg update-repo
	sudo eopkg upgrade
	sudo eopkg install dpkg
	sudo eopkg install -c system.devel
	sudo eopkg install binutils

3/ after installed in a successful manner ! type

	sudo systemctl reboot

4/ after boot: download any .deb file from internet then open terminal again and
 go to your file location using

	pwd
	cd ~/Downloads
	cd .. 	[use this to back previous directory]
	mkdir mydeb2eopkg
	cp <your deb file name.deb> mydeb2eopkg   [it will copy that deb file into mydeb2eopkg directory/folder !!!remove<>!!!]
	cd mydeb2eopkg  [to go in mydeb2eopkg directory]
	sudo ar -xv <your deb file name.deb>

it will look like this:
	x - debian-binary
	x - control.tar.xz
	x - data.tar.xz [or x - data.tar.gz]

5/ now , Create a data directory and unpack your data tar-archive there:
  
	mkdir data
	cp data.tar.xz data
	tar -xvf data.tar.xz or tar -xf data.tar.xz

Now inside the data directory there will be directories usr, bin, lib, etc.
Next, you spread the entire structure along similar paths of your distribution. [JUST COPY PASTE !] 

MY ADVICE TO RUN TWO SIDE BY SIDE FILE MANAGER AS ROOT PRIVILAGE 
FRIST ONE IN THAT DATA DIRECTORY [STEP--5] AND 2ND FILE MANAGER TO MATCH WITH THE SYSTEM PATH FORM FOLLOW PATH
IN DATA DIRECTORY!

[!!!PLEASE CAREFUL IN THIS STEP!!!]

6/ ENJOY LINUX [SOLUS LINUX] if you like rate me.... :)
