# ChatVRM

ChatVRMはブラウザで簡単に3Dキャラクターと会話ができるデモアプリケーションです。

VRMファイルをインポートしてキャラクターに合わせた声の調整や、感情表現を含んだ返答文の生成などを行うことができます。

ChatVRMの各機能は主に以下の技術を使用しています。

- ユーザーの音声の認識
    - [Web Speech API(SpeechRecognition)](https://developer.mozilla.org/ja/docs/Web/API/SpeechRecognition)
- 返答文の生成
    - [ChatGPT API](https://platform.openai.com/docs/api-reference/chat)
- 読み上げ音声の生成
    - [Koemotion/Koeiromap API](https://koemotion.rinna.co.jp/)
- 3Dキャラクターの表示
    - [@pixiv/three-vrm](https://github.com/pixiv/three-vrm)


## デモ

Glitchでデモを公開しています。

[https://chatvrm.glitch.me](https://chatvrm.glitch.me)

## 実行
ローカル環境で実行する場合はこのリポジトリをクローンするか、ダウンロードしてください。

```bash
git clone git@github.com:pixiv/ChatVRM.git
```

必要なパッケージをインストールしてください。
```bash
npm install
```

パッケージのインストールが完了した後、以下のコマンドで開発用のWebサーバーを起動します。
```bash
npm run dev
```

実行後、以下のURLにアクセスして動作を確認して下さい。

[http://localhost:3000](http://localhost:3000) 


---

## ChatGPT API

ChatVRMでは返答文の生成にChatGPT APIを使用しています。

ChatGPT APIの仕様や利用規約については以下のリンクや公式サイトをご確認ください。

- [https://platform.openai.com/docs/api-reference/chat](https://platform.openai.com/docs/api-reference/chat)
- [https://openai.com/policies/api-data-usage-policies](https://openai.com/policies/api-data-usage-policies)


## SHARE VOXと連携

音声を使う場合は、ローカルでSHARE VOXを同時に起動してください。

https://www.sharevox.app/

<img width="1141" alt="スクリーンショット 2024-04-15 23 12 45" src="https://github.com/kururu/ChatVRM/assets/909549/9b691916-1b86-4ad7-b896-3e39e5b620da">

## BGMを流す場合

BGMは左上のaudioタグを調整してください。

音量はデフォルトで中ぐらいになっています。

音声ファイルは、デフォルトでは
public/class-coffee.mp3
に入っています。

<img width="1254" alt="スクリーンショット 2024-04-15 23 07 40" src="https://github.com/kururu/ChatVRM/assets/909549/1e03a36c-6e0b-4815-805e-aefe04abbbdc">

## デモ動画

ブラウザで実行したときの様子はこちらです。

[![alt設定](https://github.com/kururu/ChatVRM/assets/909549/2fa68169-ac85-43b3-9214-2ebecac8de3d)](https://www.youtube.com/watch?v={zuA4u-NkCT4})
