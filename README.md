# manage-hatenablog

## セットアップ
[参考サイト1](https://zenn.dev/m_yamashii/articles/post-blog-using-github-actions)
※ リンク先のHATENA_API_KEYは　はてなブログの「設定/アカウント設定/APIキー」より確認

[参考サイト2](https://tanabebe.hatenablog.com/entry/2020/07/06/080000)

基本は参考サイト2の内容をもとにセットアップ（元々あった記事を取得する場合は参考サイト2の方法で）
### 参考サイト1からの変更点
.envファイルが存在しないので
```
vim .env
```
等で作成

<br>
<br>

Dckerfileを以下に変更
```
FROM golang

RUN go install github.com/x-motemen/blogsync@latest

ENTRYPOINT [ "blogsync" ]
```
