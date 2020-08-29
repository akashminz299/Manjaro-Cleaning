### 1. Clean pkg cache

#### A. List cache directory & Check size
```
  ls /var/cache/pacman/pkg/ | less 
  du -sh /var/cache/pacman/pkg/
```
#### B. Remove not installed cache packages
```sudo pacman -Sc```

#### C. Remove all cache packages
```sudo pacman -Scc```

### 2. Clean cache packages automatically using (paccache)

#### A. Download
```sudo pacman -S pacman-contrib```

#### B. Run
```paccache -r```

### 3.Remove unused packages (orphan)

#### A. List orphan packages
```sudo pacman -Qtdq```

#### B. Remove orphan packages
```sudo pacman -R $(pacman -Qtdq)```

### 4. Clean cache from home directory

#### A. List cache directory & Check size
```
  ls ~/.cache/ | less 
  du -sh ~/.cache/
```

#### Remove 
```rm -rf ~/.cache/* ```

### 5. Deleting not required configuration files

#### A. Goto
```/home/.config/```
And
```/home/.local/share/```
Delete all not required configurations. But be carefull while deleting.
