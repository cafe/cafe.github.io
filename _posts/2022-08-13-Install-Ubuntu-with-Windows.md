# Windows系统下安装Ubuntu

## 安装Ubuntu几种形式

- WSL：在Win中使用命令行较方便，图形界面支持度不友好（需要MobaXTerm等工具，软渲染性能弱）
- U盘直装：常规方式，可以装双系统或直接格式化删除Windows再装
- 使用wubi：无须分区、格式化硬盘，直接装在Windows相同的盘上，双系统启动。

选择wubi好处是无须U盘，安装简单，亦可体验到完整Ubuntu系统，且同时保留Windows系统以备不时之需。

## Wubi安装Ubuntu

- [GitHub](github.com/hakuna-m/wubiuefi/releases)下载wubi
- 下载对应系统iso文件（如通过官网或[异次元软件世界](https://dl.iplaysoft.com/files/5700.html)->点击页面`选择下载地址`），放在上述wubi工具同一个文件夹内
- 安装时选择了支持最大选择256GB（最大数值可能与当前的硬盘空闲大小有关），在wubi界面可以直接设置一个简单短小的Linux用户密码方便使用
- 安装好后，在Windows中下载安装easybcd工具，调整系统启动顺序，可将Ubuntu设为默认启动项。（注意：使用easybcd是比较危险的操作，千万不要删除启动项）
- 在Ubuntu的Software & Updates程序中选择一个国内的镜像（这里选择了nju.edu.cn)，可以大大加快软件和系统更新时的下载速度。
- 安装各种必备软件：[Rime输入法](https://github.com/cafe/wubi98/tree/master/Ubuntu)、vs code等
