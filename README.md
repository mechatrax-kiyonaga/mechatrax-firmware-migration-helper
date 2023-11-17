# mechatrax-firmware-migration-helper
raspberrypi-bootloader から raspi-firmware への移行を支援するパッケージです。  

## 提供ファイル
次のファイルがパッケージに含まれています。

### /usr/share/doc/mechatrax-firmware-migration-helper/copylight
パッケージに含まれるファイルの著作権を記述したファイルです。

## 設定
インストール時に次のファイルおよびディレクトリが変更されます。

### /etc/fstab
/boot を /boot/firmware に置換します。

### /boot/cmdline.txt
/boot/firmware/cmdline.txt のシンボリックリンクです。

### /boot/config.txt
/boot/firmware/config.txt のシンボリックリンクです。

### /boot/overlays
/boot/firmware/overlays のシンボリックリンクです。

### /boot/firmware/cmdline.txt
/boot/cmdline.txt から移動されます。

### /boot/firmware/config.txt
/boot/config.txt から移動されます。

### /boot/firmware/overlays
/boot/overlays から移動されます。

