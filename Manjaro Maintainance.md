### 1. Clean pkg cache

#### List cache directory & Check size
```
  ls /var/cache/pacman/pkg/ | less 
  du -sh /var/cache/pacman/pkg/
```
#### Remove not installed cache packages
```sudo pacman -Sc```

#### Remove all cache packages
```sudo pacman -Scc```

### 2. Clean cache packages automatically using (paccache)

#### Download
```sudo pacman -S pacman-contrib```

#### Run
```paccache -r```

### 3. Remove unused packages (orphan)

#### List orphan packages
```sudo pacman -Qtdq```

#### Remove orphan packages
```sudo pacman -R $(pacman -Qtdq)```

### 4. Clean cache from home directory

#### List cache directory & Check size
```
  ls ~/.cache/ | less 
  du -sh ~/.cache/
```

#### Remove 
```rm -rf ~/.cache/* ```

### 5. Deleting not required configuration files

#### Goto
```/home/.config/```
And
```/home/.local/share/```
Delete all not required configurations. But be carefull while deleting.
