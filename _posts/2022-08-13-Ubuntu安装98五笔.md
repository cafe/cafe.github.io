
# Ubuntu 20.04: Install Wubi98

## Links

All the following resources => [repo](https://github.com/cafe/wubi98)

1. [Official site: 98wubi](http://www.98wubi.com/zhinan.html)
2. [Resources](http://98wb.ysepan.com/)
3. [Instructions](https://www.bilibili.com/video/BV1y3411H78p)

## Steps
- Download files `Ubuntu-22.04-LTS.tar.xz`, `font-98wb.tar.xz` from link(2) (folder "Mac-Linux-iOS" and "拆分/超集字体")
- Follow instructions of link(3)

## Notes
- 如果配置好之后在vscode里无法切换到Rime，卸载从snap商店安装的vscode，按[微软官方说明](https://code.visualstudio.com/docs/setup/linux)使用其它方式安装vscode即可
- 默认四码直接出字，要更改此设置，修改`~/.config/ibus/rime`目录下的`wubi98_dz.schema.yaml`（单字设置）和`wubi98_ci.schema.yaml`（词组设置）文件，将`enable_completion`全设为`false`即可。并将这2个文件复制到`~/.config/ibus/rime/build`替换该目录下同名文件。最后点击右上角输入法状态，选择“部署”即可。
