# 環境構築

## 実行環境

### Xcode
```
$ xcode-select --install
```
### Homebrew インストール
```
$ ruby -e "$(curl -fsSL https://raw.github.com/Homebrew/homebrew/go/install)"
$ brew doctor
```

### git インストール
```
```

### home-brew cask インストール
```
$ brew install caskroom/cask/brew-cask
```

### アプリケーションのインストール先を指定
```
$ echo 'export HOMEBREW_CASK_OPTS="--appdir=/Applications"' >> ~/.bash_profile
```

## パッケージの管理

## homebrew-bundle で管理する
```
# brewにbundleコマンドが使えるようにする
$ brew tap Homebrew/bundle
# homebrewのGemfileみたいなファイルを作る
$ touch Brewfile
```


git@github.com:kiyomizu/Brewfile.git

### Brewfileの作成
```
cask_args appdir: '/Applications'
tap 'caskroom/cask'
cask 'google-chrome'
cask 'firefox', args: { appdir: '/Applications' }
```

> HomebrewでインストールしたパッケージのBrewfileを作成したい場合は `$ brew bundle dump` でOK

## アップグレード確認
```
$ brew bundle check
```

## 参考
https://github.com/caskroom/homebrew-cask/blob/master/CONTRIBUTING.md#adding-a-cask
