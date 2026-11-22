<div align="center">
MangoWM With Noctalia Shell, and Noctalia Greeter For CachyOS.
</div>

> [!IMPORTANT]
> READ INSTALLER FILE TO SEE WHAT GETS INSTALLED. Fork This Repo, and Remove Stuff You Don't Need Or If You Want To Add Something.

_____________________________________________________________________________________________________________________

## Step 1: Install MangoWM, Noctalia Shell, and Noctalia Greeter Along With Some Useful Apps:

```shell
git clone https://github.com/kitkat6464/MyConfigs.git
```

```shell
cd MyConfigs
```

```shell
chmod +x cachy-setup
```

```shell
./cachy-setup
```

_____________________________________________________________________________________________________________________

## Step 2: Setup Secondary Drive:

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
