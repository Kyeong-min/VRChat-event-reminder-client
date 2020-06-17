VRChat event reminder
=====================

- [ダウンロード (Alpha)](https://github.com/Kyeong-min/VRChat-event-reminder-client/releases/tag/alpha)

このアプリは、VRChatで開催される、様々にイベントに忘れずに参加できるようにお助けします。

指定されたイベントが開催される前に、Windows toast notificationおよび、VR HMD上でオーバーレイでお知らせします。

# 現在当アプリはαテスト版です。

αテスト版では、下記機能をサポートいたしません。
- SteamVR起動時、Overlay表示のためのアプリが自動で起動されません。
  - NotificationBroker/NotificationBroker.exeを手動で起動してください。
- インストーラ
  - α版では、圧縮ファイルの形で提供されます。
- イベントリストのソート、検索など

# このアプリをお使いになるためには、下記の条件を満たす必要があります。

## 必須
- ウィンドウズ10 64ビット
- ASP .NET Core Runtime 3.1.5 [ダウンロード](https://download.visualstudio.microsoft.com/download/pr/6818f1f7-75de-43e5-9202-2b328ca127f7/039edc4bab29e5af63ed618e59f82fad/aspnetcore-runtime-3.1.5-win-x64.exe)

## オプション
- Valve index、HTC Vive、Oculus、Windows MR など、SteamVRをサポートするVRハードウェア
- SteamVR

````
VRハードウェアおよび、SteamVRがインストールされていない環境では、Windows toast notificationを通じてのみ、イベントの開催をお知らせできます。
````

# 簡単なHow to use.
1. ダウンロードしたalpha.zipファイルを適当な位置に解凍してください。
2. aspnetcore-runtime-3.1.5-win-x64.exeを起動し、指示に従い、ランタイムをインストールします。
   - インストール済みであれば、インストールする必要はありません。
3. VRChatEventReminderフォルダーのVRChatEventReminder.exeファイルを実行してください。
4. ウェブブラウザーを立ち上げ、http://localhost:5000を入力し、接続してください。Chrome、Firefox、Edgeなどがおすすめです。
![01](image/jp/01.JPG)
    1. 今日開催が予定されたイベントのリストです。
    2. 現在進行中のイベントのリストです。
    3. お知らせ対象イベントのリストです。
5. 左のメニューから、イベントリストを選択し、参加したいイベントのチェックボックスをクリックし、チェックを入れてください。
![02](image/jp/02.JPG)
   - 終了または、開催済みのイベントは、チェックを入れることができません。
6. すると、イベントが開催される前に、イベントが始まることを知らせるアラームが見れます。

## VR HMDでアラームを見るために
1. NotificationBroker/NotificationBroker.exeファイルを起動してください。
   - この際、SteamVRが起動中でない場合、SteamVRが自動で起動されます。
2. イベントが開催される前に、イベントの開催を知らせるアラームをVR HMD上で見れます。
3. SteamVR Dashboardから、VRChat event reminderのダッシュボードを通じて、アラームの見え方を設定できます。
![gif01](image/001.gif)
4. オーバーレイの表示位置、スケール、透明度、表示時間を設定し、Show sample notificationボタンをインタラクティブ(大体の場合、コントローラのトリガーボタンまたは、HMDのセレクトボタン)することで、テストできます。
![gif02](image/002.gif)

# このアプリの不具合について
どういう操作を行い、どの問題が発生したかを私に教えてくださると、テストおよび、開発において、大変な助かりとなります。

下記の中から、楽な方法を利用して、私に教えてください。

- ツイッター @isHATENA にて、DMを送ってください。
- [Github repository](https://github.com/Kyeong-min/VRChat-event-reminder-client/issues)にて、issueを切ってください。

私にお知らせの際、ログファイルを一緒にいただくと大変助かります。
- VRChatEventReminder\log\ の中のすべての *.log ファイル
- NotificationBroker\logger.log ファイル

# About
- 開発: HATENA([@isHATENA](https://twitter.com/isHATENA))
- アイコン: コールマン＆アルナイル([@callman_alnair](https://twitter.com/callman_alnair))

## VRChatイベント開催情報の情報取得元明記
- VRChat イベントカレンダー
  - https://sites.google.com/view/vrchat-event
  - 運営管理者 カッコウ ([@nest_cuckoo_](https://twitter.com/nest_cuckoo_))
- 한국 VRChat 이벤트 캘린더
  - https://sites.google.com/view/vrcevent-kr
  - 運用管理者 R3C0D3r([@r3c0d3r](https://twitter.com/r3c0d3r))

## VRChatイベント開催情報の責任範囲について
- 各イベント開催情報の権利は、原則、各イベント開催情報の運営管理者が保持します。
- イベント開催情報の登録、修正の依頼は、各イベント開催情報の運営管理者にてお願いいたします。
- 本アプリの不具合などの問題は、開発者であるHATENAにてお願いいたします。