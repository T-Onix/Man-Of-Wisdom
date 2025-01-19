### ~={red}Useful Command For Linux=~

Run ls then exit from terminal :
```shell
exec ls
```

Run the command in other shell then exit :
```shell
(ls)
```

Show error when echo have error :
```shell
set -u
```

Dont show error in echo :
```shell
set +u
```

Run last command typed :
```shell
!!
```

Find the command with this name and run it :
```shell
!command
```

Find the word that typed :
```shell
!?word
```

Search for some command related to word :
```shell
man -k word
```

Sort the list :
```sh
ls | sort
```

Show the line's :
```sh
ls | wc -l
```

Write ls in the file :
```sh
ls > file.txt
```

Cat the txt then with with ctrl + d cat nextone :
```sh
cat file.txt - file.txt1 
```

Split file.txt file line's by 2 and creat seprated file :
```sh
split -l2 file.txt
```

show last 10 line's and wait for info (~={red}Useful for Logfiles or live files=~) :
```sh
tail -f file.txt
```

Print the file :
```sh
pr file.txt
```

Show the line numbers :
```sh
nl file.txt or cat -n 
```

Show 10 line's in every paragraf :
```sh
fmt -w10 file.txt
```

For sorting numbers :
```sh
sort -n file.txt
```

Delete duplicated word's :
```sh
sort file.txt | uniq
```

Show duplicated word's :
```sh
uniq -c
```

Replace a with b :
```sh
cat file.txt | tr 'a' 'b'
```

Replace a with b :
```sh
sed 's/a/b' file.txt
```

Replace all the a with b :
```sh
sed 's/a/b/g' file.txt
```

Get a backup of file.txt then copy to file1.txt :
```sh
cp -b file.txt file1.txt
```

Make several directories :
```sh
mkdir -p dir/dir1
```

Remove the whole dir :
```sh
rm -r dir
```

Get ls of file'a that strat's with 'a' :
```sh
ls *a
```

ls that file are a to z :
```sh
ls [a-z]*
```

Change the time of file :
```sh
touch -d "5 nov 2005"
```

Show types of file :
```sh
file song.mp3
```

Write stderr to file :
```sh
ls 2> file.txt
```

> [! note]
> ~={red}1>=~ : for stdout and default one
> ~={red}2>=~ : for stderr
> ~={red}0>=~ : for stdin

Append to a file :
```sh
>>
```

Write stdout and stdin :
```sh
&>
```

First list will be echo then ls :
```sh
ls | xargs echo list: 
```

Write ls in file then show it :
```sh
ls | tee file.txt
```

Run the stoped proccess in the background :
```sh
bg
```

Show the background proccess :
```sh
fg
```

Show the background proccess :
```sh
jobs
```

Show background proccess in terminal :
```sh
fg %1
```

Show all the running proccess :
```sh
ps -aux
```

Give system hardware to a command (~={red}-20 = highest=~ , ~={green}19 = lowest=~): 
```sh 
nice -n 11 command
```

Change the nice number : 
```sh
renice -n 4 proccessid 
```

Find hi in file :
```sh 
grep hi file.txt
```

Show number of line's :
```sh
egrep -n hi file.txt 
```

Add new user :
```sh
adduser darlin
```

Lock user that can't login :
```sh
usermod -L darlin
```

Unlock user :
```sh
usermod -U darlin 
```

Delete user :
```sh
userdel darlin
```

Delete user with it's directory :
```sh
userdel -r darlin
```

Add darlin to sudo group :
```sh
usermod -aG sudo darlin
```

Set time to doing smt :
```sh
crontab -e
```

Run some command today after 2 min :
```sh 
at now + 2 min
```

Show current jobs :
```sh
atq
```

Delete job :
```sh
atrm number
```

Set timezone :
```sh
tzselect
```

Change ip address :
```sh
ifconfig 'interface/name' ip
```

Extract gz  file's :
```sh
tar xzvf file.tar.gz
```

Extract bz2 file's :
```sh
tar xjf file.tar.bz2 
```

Change DNS in arch : 
```sh
sudo vim /etc/resolv.conf
```

Show connected connection's :
```sh
nmcli
```

File can't be modified anymore :
```sh
chattr +i file.txt
```

Show active internet connection's :
```sh
netstat -antup
```

List kernel module's :
```sh
lsmod
```

Add or remove module's from kernel :
```sh
modprobe
```

Make symbolik folder :
```sh
ln -s
```

Flash the ip address : 
```sh
ip addr flash dev Interface/Name
```

Add new ip :
```
dhclient Interface/Name
```