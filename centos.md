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
