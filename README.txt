关于本网站
======================

网站名称：逻辑谬误
网站内容：收录常见的逻辑错误
源码语言：reStructuredText
源码托管：GitHub
网页托管：readthedocs

编译工具
----------------------
本网站使用Sphinx工具链进行编译，使用bizstyle主题（完美兼容手机等小屏设备，且不使用托管在google等网站的字体、脚本）。

安装了pip的Windows、Linux操作系统均可以使用以下命令安装Sphinx：
pip install sphinx

openSUSE Linux的官方软件源已经包含了Sphinx软件包，可以使用
sudo zypper in python-Sphinx （python2版本） 或者
sudo zypper in python3-Sphinx （python3版本） 进行安装。

最新版本的Sphinx已经内部包含bizstyle主题，若正使用旧版本Sphinx，可以使用以下命令安装bizstyle主题：
pip install sphinxjp.themes.bizstyle

考虑到mathjax的外挂js、字体体积太大，严重影响网页打开速度，本站设置使用pngmath解决潜在的数学公式渲染需求。因此编译含有数学公式的源代码需要安装LaTeX（推荐TeXLive发行版）。不过在数学公式上本网站优先考虑使用unicode字符、上标下标等功能来实现简单数学式（主要是逻辑式）的功能。这样可以减少图片的使用，也可以避免小屏设备显示中数学式图片被单行显示出现放大过度的状况。因此目前本站源码中尚未使用任何需要pngmath输出图片公式的源码。

编译方法
----------------------
Windows操作系统：
.\make.bat html

Linux操作系统：
make html
