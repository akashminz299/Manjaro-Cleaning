### Clean pkg cache

#### 1. List cache directory & Check size
```
  ls /var/cache/pacman/pkg/ | less 
  du -sh /var/cache/pacman/pkg/
```
#### 2. Remove not installed cache packages
```sudo pacman -Sc```

#### 3. Remove all cache packages
```sudo pacman -Scc```

### Clean cache packages automatically using (paccache)

#### 1. Download
```sudo pacman -S pacman-contrib```

#### 2. Run
```paccache -r```

### Remove unused packages (orphan)

#### 1. List orphan packages
```sudo pacman -Qtdq```

#### 2. Remove orphan packages
```sudo pacman -R $(pacman -Qtdq)```

### Clean cache from home directory

#### 1. List cache directory & Check size
```
  ls ~/.cache/ | less 
  du -sh ~/.cache/
```

#### 2. Remove 
```rm -rf ~/.cache/* ```

### Deleting not required configuration files

#### 1. Goto
```/home/.config/```
And
```/home/.local/share/```
Delete all not required configurations. But be carefull while deleting.
