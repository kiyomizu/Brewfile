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
$  brew install git
```

### brew update
```
$ brew update
```

### home-brew cask インストール
```
$ brew install caskroom/cask/brew-cask
```

### アプリケーションのインストール先を指定
```
$ echo 'export HOMEBREW_CASK_OPTS="--appdir=/Applications"' >> ~/.bash_profile
```

### brew-fileインストール
```
$ brew tap rcmdnk/file
$ brew install brew-file
```

### git Brewfileをセットする
```
$ brew file set_repo -r git@github.com:kiyomizu/Brewfile
$ brew file init
```

### Brewfileの編集
```
$ brew file casklist
$ brew file edit
```

### アプリケーションのアップデート
```
$ brew file cask_upgrade -C
# 古いバージョンも残す場合は
$ brew cask update
S```

## 参考
https://github.com/caskroom/homebrew-cask/blob/master/CONTRIBUTING.md#adding-a-cask
