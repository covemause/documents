よく忘れるコマンド類

## バージョン情報
```
cat /etc/redhat-release 
```

## ファイヤーウォール
```
firewall-cmd --list-all # 確認
firewall-cmd --zone=public --add-port=443/tcp --permanent # ポート指定
firewall-cmd --zone=public --add-service=http --permanent # サービス指定
firewall-cmd --reload # 反映
```

## ネットワーク
```
nmcli device show # 接続情報
nmcli con mod DeviceNo ipv4.addresses "192.168.24.127/24 192.168.24.2" # IPアドレスの変更 ※DeviceNo = enp01などのデバイス名に置換
nmcli con mod DeviceNo ipv4.method auto # DHCP
nmcli con mod DeviceNo connection.autoconnect "yes" # 自動接続
nmcli con down DeviceNo # 停止
nmcli con up DeviceNo # 起動
```
