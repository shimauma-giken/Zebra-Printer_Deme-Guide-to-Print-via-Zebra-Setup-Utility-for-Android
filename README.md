# Zebra-Printer_Deme Guide to Print via Zebra Setup Utility for Android
 速習_Zebra Setup Utility for Android

#### インストールすべき基本ソフトを理解する

1. ZDesigner driver version 10 ★
1. Zebra Printer Setup Utilities for Windows ★
1. Zebra Designer Professional ★
1. Zebra Printer Setup Utilities for Android ★
1. Zebra Printer Setup Utilities for Windows 



#### プリンタを初期化する方法を学ぶ

- パソコン操作 (Zebra Setup Utilities for Windows)  
https://github.com/shimauma-giken/Zebra-Printer-How-to-Completely-Wipe-Data-and-Factory-Install-Link-OS-Priner?tab=readme-ov-file#%E3%83%91%E3%82%BD%E3%82%B3%E3%83%B3%E6%93%8D%E4%BD%9C-zebra-setup-utilities-for-windows  

        E.g
        ~PMXXRAJ204201739,0


#### プリンタの設定（Bluetooth + デモ用設定）

1. ZSU for Win > Open Communication with Printer
1. 下記コマンド入力 > Send To Printer

    <pre>
    -- Set Demo Environment
    ! U1 setvar "device.languages" "zpl"
    ! U1 setvar "power.inactivity_timeout" "0"
    ! U1 setvar "device.pnp_option" "zpl"
    -- Set Bluetooth
    ! U1 setvar "bluetooth.enable" "on"
    ! U1 setvar "bluetooth.discoverable" "on"
    ! U1 setvar "bluetooth.minimum_security_mode" "1"
    -- Connect to Zatar
    ! U1 setvar "ip.dhcp.enable" "on"
    ! U1 setvar "wlan.ip.protocol" "dhcp"
    ! U1 setvar "wlan.essid" "Zatar"
    ! U1 setvar "wlan.leap_mode" "off"
    ! U1 setvar "wlan.kerberos.mode" "off"
    ! U1 setvar "wlan.encryption_mode" "off"
    ! U1 setvar "wlan.8021x.enable" "off"
    ! U1 setvar "wlan.operating_mode" "infrastructure"
    ! U1 setvar "wlan.allowed_band" "all"
    ! U1 setvar "wlan.international_mode" "off"
    ! U1 setvar "wlan.wpa.authentication" "psk"
    ! U1 setvar "wlan.wpa.enable" "on"
    ! U1 setvar "wlan.wpa.psk" "3FD3B4084C9A70E65AAC31BCF45C1707EB6F91B62BADF7EA27B0E0C7AEFB3717"
    -- Reboot
    ! U1 do "device.reset" ""
    ~HS
    </pre>


#### ZSUの再起動

1. ZSUを再起動
1. [プリンタ名（ZPL)]を選択する。


#### プリンタの設定（用紙）

1. Zebra Setup Utilities > Configure Printer Settings
    - Width, Height
    - Speed, Darkness
    - Media Type, Use of Feed Button

1. Open Printer Tools > Calibrate Media > Calibrate

※ラベルが止まらない場合はMedia Typeを再確認すること


#### 日本語の登録 (Windows Driver)

https://github.com/shimauma-giken/Zebra-Printer-Add-Japanese-Font-to-Windows-Driver-to-Utilize-in-Zebra-Designer

#### 簡易なラベルをデザイン・作成できるようになる

1. Zebra Designer Professional 起動
1. プリンタを選択し、初期設定する。
1. 用紙をデザインする
1. 印刷（USB経由）

#### 印刷データファイルの作成

1. Zebra Designer Professional > 印刷 (ファイルに出力する)
1. Android 端末内の任意のフォルダに保存

#### Android端末とペアリング

1. Zebra Setup Utilities for Android 起動
1. NFC タッチペアリング

#### プリンタの設定（用紙）
※ PCで設定していない場合は再設定
1. ZSU for A > 用紙設定
1．> プリンタの動作 > 用紙をキャリブレート


#### ZSU for A から印刷

1. 使用可能なファイル > 保存したファイルを選択

#### 応用（時間があれば）


