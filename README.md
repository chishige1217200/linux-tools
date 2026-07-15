# linux-tools

Linux用の便利スクリプト群です。

## ファイル構成

### deepcool/
- `deepcool-digital-linux.service`
  - `/opt/deepcool/deepcool-digital-linux`を実行します。
  - [deepcool-digital-linux](https://github.com/Nortank12/deepcool-digital-linux)を配置してください。

### nvidia/
- `nvidia-fan-control.service`
  - NVIDIA GPUのファン制御を有効にし、目標ファン速度を60%に設定します。
  - `nvidia-settings`を使用してXディスプレイ(:0)に対して設定します。

- `nvidia-pl-limit.service`
  - NVIDIA GPUの電力制限（Power Limit）を250Wに設定します。
  - `nvidia-smi -pl 250`を実行します。

### wacom/
- `unload-wacom-driver.service`
  - Wacomタブレットドライバーをアンロードします（`rmmod wacom`）。
  - `locao-fs.target`後に実行

