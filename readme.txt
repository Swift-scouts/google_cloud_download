
登录到google cloud界面，选中要下载的目录，点击下载，会提示使用 gsutil 命令行工具，并提供命令行复制

警告：某些 Linux 发行版中预安装了另一个名为 gsutil 的工具（由 GrandStream BudgeTone 提供）。如果您运行此命令（而不是 Cloud Storage gsutil），它可能会输出类似于 "Choose one of -b, -d, -e, or -r to do something" 的错误消息。如果发生这种情况，您可以在 PATH 环境变量中将 Cloud Storage 版 gsutil 移到前面，或者，您也可以在运行 Cloud Storage gsutil 时指定完整路径（例如 /home/users/joan/gsutil/gsutil ls）
1，安装
sudo apt install pip
pip install gsutil
export PATH=$PATH:/home/ipfsbit/.local/bin  临时添加路径
echo "export PATH=$PATH:/home/ipfsbit/.local/bin" >>~/.bashrc
source ~/.bashrc
nohup gsutil -m cp -r "gs://xxx/xxx"  ./ &


