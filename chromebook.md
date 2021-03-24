# chromebook

```
sudo apt update
sudo apt upgrade -y
```

## Snap

いろいろ制限が多いうえ、速度が遅い。対処している時間で普通通りやったほうが早い。よって断念。

## apt

### vscode

[Visual Studio Code on Linux](https://code.visualstudio.com/docs/setup/linux)

```
wget -qO- https://packages.microsoft.com/keys/microsoft.asc | gpg --dearmor > packages.microsoft.gpg
sudo install -o root -g root -m 644 packages.microsoft.gpg /etc/apt/trusted.gpg.d/
sudo sh -c 'echo "deb [arch=amd64,arm64,armhf signed-by=/etc/apt/trusted.gpg.d/packages.microsoft.gpg] https://packages.microsoft.com/repos/code stable main" > /etc/apt/sources.list.d/vscode.list'

sudo apt install apt-transport-https
sudo apt update
sudo apt install code
```

### Node.js

[Node.js Binary Distributions](https://github.com/nodesource/distributions/blob/master/README.md)

```
curl -fsSL https://deb.nodesource.com/setup_current.x | sudo -E bash -
sudo apt install -y nodejs
```

### Git

```
git config --global user.email "メールアドレス"
git config --global user.name "名前"
```
