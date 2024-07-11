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

[return](../README.md)

## Hydra
```
hydra -L user.lst -P pass.lst -t 8 10.0.0.5 ftp
```
