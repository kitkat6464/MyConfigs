<div align="center">
MangoWM With Noctalia Shell and Noctalia Greeter For EndeavourOS.
</div>

> [!IMPORTANT]
> READ INSTALLER FILE TO SEE WHAT GETS INSTALLED. Fork This Repo and Remove Stuff You Don't Need Or If You Want To Add Something.

_____________________________________________________________________________________________________________________

## Step 1: Install MangoWM and Noctalia Greeter From The AUR (Run This If You Installed With No Desktop)

> [!IMPORTANT]
> For Security Reasons, WE WILL NOT AUTOMATE AUR PACKAGE INSTALLS IN THE AUTOMATED SETUP. THEY MUST BE INSTALLED MANUALLY.

- MangoWM:
```shell
yay -S mangowm
```

- Noctalia Greeter:
```shell
yay -S noctalia-greeter
```
_____________________________________________________________________________________________________________________

## Step 2: Install Noctalia Shell Along With Some Useful Apps:

```shell
curl -fsSL https://raw.githubusercontent.com/kitkat6464/MyConfigs/refs/heads/mango/Required-Setup | sh
```

_____________________________________________________________________________________________________________________

## Step 3: Setup Secondary Drive:

```shell
sudo mkdir /mnt/games
```

> [!IMPORTANT]
> Use This Command To Find The Drive's UUID.

```shell
lsblk -f
```

> [!IMPORTANT]
> Modify fstab Carefully.

```shell
sudo nano /etc/fstab
```

| Example: |
|:---:|
| UUID=YOURDRIVEUUID /mnt/games     btrfs   defaults,noatime,x-gvfs-show,compress=zstd,commit=120 0 0 |

> [!IMPORTANT]
> Now Reboot PC.

```shell
sudo reboot
```
_____________________________________________________________________________________________________________________
