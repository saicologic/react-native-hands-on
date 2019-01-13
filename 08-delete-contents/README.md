# やること
- チェックボックスをタップしたときに、アイテムを削除する
  - App.jsの修正
  - firebase.jsの修正
- Simulatorで確認
- ログの確認

# 手順
## チェックボックスをタップしたときに、アイテムを削除する

#### App.jsの修正

completeItemを追加します。

参考: [todoapp/App.js](https://github.com/saicologic/todoapp/blob/master/App.js#L85-L88)

```
  completeItem = async (item) => {
    await firebase.complteItem(item);
    await this.getItems();
  }
```

### firebase.jsの修正

参考: [todoapp/firebase.js](https://github.com/saicologic/todoapp/blob/master/firebase.js#L29-L37)


complteItemを追加します。

```

complteItem = async (item) => {
  this.firestore.collection('items').doc(item.itemId).delete()
    .then(() => {
      console.log('Document successfully deleted!');
    })
    .catch((error) => {
      console.error('Error removing document: ', error);
    });
}
```

## Simulatorで確認

![](images/delete_content.png)

## ログの確認

![](images/log.png)
