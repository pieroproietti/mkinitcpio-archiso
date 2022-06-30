mkinitcpio-archiso
sudo make install

a questo punto si dovrebbe creare LA  configurazione
per mkinitcpio.conf come la seguente:

```
MODULES=()
BINARIES=()
FILES=()
HOOKS=(base udev modconf memdisk archiso archiso_loop_mnt archiso_pxe_common archiso_pxe_nbd archiso_pxe_http archiso_pxe_nfs archiso_kms block filesystems keyboard)
COMPRESSION="xz"
#COMPRESSION_OPTIONS=()


#
git config --global core.editor "nano"
sudo localectl set-keymap it
