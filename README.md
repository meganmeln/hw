Welcome to JS/Linux (i586)
 
Use 'vflogin username' to connect to your account.
You can create a new account at https://vfsync.org/signup .
Use 'export_file filename' to export a file to your computer.
Imported files are written to the home directory.
 
localhost:~# cd ..
localhost:/# ls
bin    etc    lib    mnt    proc   run    srv    tmp    var
dev    home   media  opt    root   sbin   sys    usr
localhost:/# cd /home
localhost:/home# mkdir animals/
localhost:/home# mkdir animals/dogs
localhost:/home# mkdir animals/cats
localhost:/home# mkdir animals/fisch
localhost:/home# ls
animals
localhost:/home# cd /animals
sh: cd: can't cd to /animals: No such file or directory
localhost:/home# touch animals/dogs/pluto
localhost:/home# touch animals/cats/garfield
localhost:/home# touch animals/fish/nemo
touch: animals/fish/nemo: No such file or directory
localhost:/home# touch animals/fisch/nemo
localhost:/home# cd /tmp
localhost:/tmp# mkdir humans/
localhost:/tmp# ls
humans
localhost:/tmp# cd h
sh: cd: can't cd to h: No such file or directory
localhost:/tmp# cd
localhost:~# mv /tmp/humans /opt/home/humans
mv: can't rename '/tmp/humans': No such file or directory
localhost:~# ls
bench.py    hello.c     hello.js    readme.txt
localhost:~# ls /tmp
humans
localhost:~# mv /tmp/humans /home/humans
localhost:~# cd /tmp
localhost:/tmp# touch adam
localhost:/tmp# touch eva
localhost:/tmp# cd
localhost:~# cp /tmp/adam /home/humans
localhost:~# mv /tmp/eva /opt/eve
localhost:~# mv /opt/eve /home/humans
localhost:~# ls /humans
ls: /humans: No such file or directory
localhost:~# cd /home/humans
localhost:/home/humans# ls
adam  eve
localhost:/home/humans# cd
localhost:~# history > history.txt
