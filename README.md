# mechatrax-firmware-migration-helper
raspberrypi-bootloader から raspi-firmware への移行を支援するパッケージです。  
ソースファイルからは次のパッケージが作成されます。  
* mechatrax-firmware-migration-helper
* mechatrax-firmware-dummy

# mechatrax-firmware-migration-helper
パッケージ移行時の事前設定を行います。

## 提供ファイル
次のファイルがパッケージに含まれています。

### /usr/share/doc/mechatrax-firmware-migration-helper/copylight
パッケージに含まれるファイルの著作権を記述したファイルです。

## 設定
インストール時に次のファイルが変更されます。

### /etc/fstab
/boot 表記が /boot/firmware に置き換えられます。
/etc/fstab のバックアップファイルとして /etc/fstab.bak が作成されます。

### /boot/cmdline.txt
/boot/firmware に移動し、/boot にシンボリックリンクが作成されます。

### /boot/config.txt
/boot/firmware に移動し、/boot にシンボリックリンクが作成されます。

### /boot/overlays
/boot/firmware に移動し、/boot にシンボリックリンクが作成されます。

# mechatrax-firmware-dummy
パッケージ移行時の依存関係を解決するダミーパッケージです。

## 提供ファイル
次のファイルがパッケージに含まれています。

### /usr/share/doc/mechatrax-firmware-dummy/copylight
パッケージに含まれるファイルの著作権を記述したファイルです。
