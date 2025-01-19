#### ~={green}How to use=~ :

Install packages : 
```shell
pacman -S 
```

Update packages:
```shell
pacman -Syu
```

Remove packages :
```shell
pacman -R
```

Remove Packages with dependences : 
```shell
pacman -Rs
```

if "-Rs" Got error try this :
```shell
pacman -Rsu
```

Force to delete a package :
```shell
pacman -Rdd
```

Search for a package :
```shell
pacman -Ss
```

Search for locally installed package :
```shell
pacman -Qi
```

Delete cache :
```shell
pacman -Sc
```

Remove cache more aggresive :
```shell
pacman -Scc
```

Download a package without installing it :
```shell
pacman -Sw
```