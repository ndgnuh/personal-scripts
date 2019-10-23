# personal-scripts
personal scripts

```sh
pd=$PWD
mkdir /tmp/personal-scripts
cd /tmp/personal-scripts
wget https://raw.githubusercontent.com/ndgnuh/personal-scripts/master/PKGBUILD
makepkg -si 
cd $pd
yes | rm /tmp/personal-scripts -rf
```
