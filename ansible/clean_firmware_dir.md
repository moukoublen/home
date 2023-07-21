After some upgrades there might be *.bak files in `firmware` and `firmware/overlays` directories.

To clean those run:

```shell
sudo rm -rf /boot/firmware/*.bak
sudo rm -rf /boot/firmware/overlays/*.bak
sudo fstrim -v --all
```
