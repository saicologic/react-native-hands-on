
# やること
- Googleのアカウントを取得する
- Google Cloud Platformでプロジェクトを作成する
- ウェブアプリにFirebaseを追加で設定情報を取得する
- app.jsonに設定する

# 手順
## Googleのアカウントを取得する

## Google Cloud Platformでプロジェクトを作成する
https://console.cloud.google.com/projectcreate?previousPage=%2Fiam-admin%2Fsettings%3Fproject%3Drepro-reactnative-handson%26_ga%3D2.12973111.-1010586665.1545205546&organizationId=0

## Firebaseのプロジェクトを作成する
https://console.firebase.google.com/u/0/?hl=ja

さきほど作成した、プロジェクトを利用して、Firebaseのプロジェクトを作成します。

![](images/add_project_button.png)


1. プロジェクトを指定する
2. Firebaseを追加

![](images/add_project.png)

## ウェブアプリにFirebaseを追加で設定情報を取得する

ホーム画面のProject Overviewを開きます。最初に表示されるページです。

![](images/top.png)

![](images/firebase_webapp.png)

下記をコピペします。

- apiKey
- authDomain
- databaseURL
- projectId
- storageBucket
- messageingSenderId

## app.jsonに設定する

app.jsonに追記します。
参考: [todoapp/app.json](https://github.com/saicologic/todoapp/blob/master/app.json)

```
"extra": {
  "firebase": {
    "apiKey": "",
    "authDomain": "",
    "databaseURL": "",
    "projectId": "",
    "storageBucket": "",
    "messagingSenderId": ""
  }
},
```
