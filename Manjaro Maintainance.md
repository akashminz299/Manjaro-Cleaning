### 1. Clean pkg cache

####    a) List cache directory & Check size
```
  ls /var/cache/pacman/pkg/ | less 
  du -sh /var/cache/pacman/pkg/
```
####    b) Remove not installed cache packages
```sudo pacman -Sc```

####    c) Remove all cache packages
```sudo pacman -Scc```

### 2. Clean cache packages automatically using (paccache)

####    a) Download
```sudo pacman -S pacman-contrib```

####    b) Run
```paccache -r```

### 3.Remove unused packages (orphan)

####    a) List orphan packages
```sudo pacman -Qtdq```

####    b) Remove orphan packages
```sudo pacman -R $(pacman -Qtdq)```

### 4. Clean cache from home directory

####    a) List cache directory & Check size
```
  ls ~/.cache/ | less 
  du -sh ~/.cache/
```

####    b) Remove 
```rm -rf ~/.cache/* ```

### 5. Deleting not required configuration files

####    a) Goto
```/home/.config/```
And
```/home/.local/share/```
Delete all not required configurations. But be carefull while deleting.
