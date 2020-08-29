### 1. Installing Updates

#### To update the package database and update all packages on the system.

```sudo pacman -Syu```
    
#### To force a full refresh of the package database and update all packages on the system.

```sudo pacman -Syyu```

### 2. Installing Packages

#### Best practise
    
```sudo pacman -Syu <package name>```

#### From local repo ( /var/cache/pacman/pkg/<pkg name> )

```sudo pacman -U /var/cache/pacman/pkg/<pkg-name>```

### 3. Removing Package

#### Basic syntax

```sudo pacman -R <pkg name>```
    
#### To also remove unneeded dependencies

```sudo pacman -Rsu <pkg name>```

#### Remove without creating backup for configuration files (add n)

```
  sudo pacman -Rsun <pkg name>
  sudo pacman -Rn <pkg name>
```
