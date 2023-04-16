# electron のチュートリアル実行
https://www.electronjs.org/docs/latest/tutorial/quick-start

## ディレクトリを作成して electron をインストール

```
> mkdir my-electron-app && cd my-electron-app
> npm init

> npm install --save-dev electron
```

## 実行コマンド（package.json に記載）

```
  "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1",
    "start": "electron ."
  },
```

```
npm start
```

### npx から実行する場合

```
npx electron .
```

## パッケージ化して配布

### Electron Forge のインストール

パッケージ化して配布するために必要なライブラリ

```
npm install --save-dev @electron-forge/cli
npx electron-forge import
```

### 配布可能ファイルを作成

```
npm run make
```