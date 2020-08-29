### Installing Updates

#### 1. To update the package database and update all packages on the system.

```sudo pacman -Syu```
    
#### 2. To force a full refresh of the package database and update all packages on the system.

```sudo pacman -Syyu```

### Installing Packages

#### 1. Best practise
    
```sudo pacman -Syu <package name>```

#### 2. From local repo ( /var/cache/pacman/pkg/<pkg name> )

```sudo pacman -U /var/cache/pacman/pkg/<pkg-name>```

### Removing Package

#### 1. Basic syntax

```sudo pacman -R <pkg name>```
    
#### 2. To also remove unneeded dependencies

```sudo pacman -Rsu <pkg name>```

#### 3. Remove without creating backup for configuration files (add n)

```
  sudo pacman -Rsun <pkg name>
  sudo pacman -Rn <pkg name>
```
