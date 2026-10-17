# rcs-link

LINE などのアプリから RCS / SMS のチャット画面へスムーズに遷移するためのリダイレクト用ページです。

## 概要

Androidの LINE アプリ内の制約で `sms:` スキームが正しく起動しない問題を回避するため、Web ページ経由で端末のメッセージアプリを起動します。電話番号を直接コード上に残さないよう、URL パラメータで受け取る構成にしています。

送信相手がiOSの場合は以下の形式を推奨します。（+81XXXXXXXXXXの箇所には遷移させたいユーザーの電話番号）

```text
sms://+81XXXXXXXXXX
```

## 使い方

以下の形式で URL を作成し、LINE 等で送信します。（+81XXXXXXXXXXの箇所には遷移させたいユーザーの電話番号）

```text
https://rcs-link.yukip02.com/?tel=+81XXXXXXXXXX&openExternalBrowser=1
```
