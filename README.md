# ACM Cheat Sheet

## PDF 下载
- [ACM Cheat Sheet (C).pdf](https://github.com/soulmachine/acm-cheat-sheet/blob/master/C/%E6%89%8B%E5%86%99%E4%BB%A3%E7%A0%81%E5%BF%85%E5%A4%87%E6%89%8B%E5%86%8C(C%E7%89%88).pdf?raw=true)
- [ACM Cheat Sheet (C++).pdf](https://github.com/soulmachine/acm-cheat-sheet/blob/master/C++/%E6%89%8B%E5%86%99%E4%BB%A3%E7%A0%81%E5%BF%85%E5%A4%87%E6%89%8B%E5%86%8C(C++%E7%89%88).pdf?raw=true)

C 文件夹下是 C 版，内容一模一样，代码是用纯 C 写的。

C++ 文件夹下是 C++ 版，内容一模一样，代码是用 C++ 写的。

Java 文件夹下是 Java 版，内容一模一样，代码是用 Java 写的。

## LaTeX 模板
本书使用的是陈硕开源的[模板](https://github.com/chenshuo/typeset)。该模板已用于陈硕所著[《Linux 多线程服务端编程：使用 muduo C++ 网络库》](http://chenshuo.com/book/)，并已出版。

这个模板制作精良，很有 taste，感谢陈硕 :)

## 在 Windows 下编译
1. 安装 TeX Live 2013（见官网：[tug.org/texlive](http://www.tug.org/texlive/)）。把 bin 目录（例如 `D:\texlive\2013\bin\win32`）加入 PATH 环境变量。
1. 安装字体。此 LaTeX 模板共使用 9 种字体，下载地址为 [pan.baidu.com/s/1gdefYiJ](http://pan.baidu.com/s/1gdefYiJ)。有的字体 Windows 自带，有的字体 Ubuntu 自带，但都不全，建议一次性安装完整字体包。
1. 安装 TeXstudio（[texstudio.sourceforge.net](http://texstudio.sourceforge.net/)）。
1.（可选）启动 TeX Live Manager，更新所有已安装的软件包。
1. 配置 TeXstudio：

    启动 TeXstudio，选择 `Options --> Configure TeXstudio --> Commands`，将 XeLaTeX 设置为 `xelatex -synctex=1 -interaction=nonstopmode %.tex`。

    选择 `Options --> Configure TeXstudio --> Build`：

    - 将 Build & View 从默认的 PDF Chain 改为 Compile & View；
    - 将 Default Compiler 从默认的 PDFLaTeX 修改为 XeLaTeX；
    - 将 PDF Viewer 改为 “Internal PDF Viewer (windowed)”，便于弹出独立预览窗口。

1. 编译。用 TeXstudio 打开 `ACM-cheat-sheet.tex`，点击界面上的绿色箭头开始编译。

    在下方窗口可看到 TeXstudio 使用的编译命令为：`xelatex -synctex=1 -interaction=nonstopmode "ACM-cheat-sheet".tex`

## 在 Ubuntu 下编译
1. 安装 TeX Live 2013（[tug.org/texlive](http://www.tug.org/texlive/)）。

    1.1 下载 TeX Live 2013 的 ISO 光盘（[tug.org/texlive/acquire-iso.html](http://www.tug.org/texlive/acquire-iso.html)）。

    1.2 挂载光盘后运行 `sudo ./install-tl` 开始安装。

    1.3 加入环境变量：

        sudo vi /etc/profile
        export PATH=$PATH:/usr/local/texlive/2013/bin/x86_64-linux
        export MANPATH=$MANPATH:/usr/local/texlive/2013/texmf-dist/doc/man
        export INFPATH=$INFPATH:/usr/local/texlive/2013/texmf-dist/doc/info

1. 安装字体。此 LaTeX 模板共使用 9 种字体，下载地址为 [pan.baidu.com/s/1gdefYiJ](http://pan.baidu.com/s/1gdefYiJ)。有的字体 Windows 自带，有的字体 Ubuntu 自带，但都不全，建议一次性安装完整字体包。
1. 安装 TeXstudio（[texstudio.sourceforge.net](http://texstudio.sourceforge.net/)）。
1. 配置 TeXstudio：

    启动 TeXstudio，选择 `Options --> Configure TeXstudio --> Commands`，将 XeLaTeX 设置为 `xelatex -synctex=1 -interaction=nonstopmode %.tex`。

    选择 `Options --> Configure TeXstudio --> Build`：

    - 将 Build & View 从默认的 PDF Chain 改为 Compile & View；
    - 将 Default Compiler 从默认的 PDFLaTeX 修改为 XeLaTeX；
    - 将 PDF Viewer 改为 “Internal PDF Viewer (windowed)”。

1. 编译。用 TeXstudio 打开 `ACM-cheat-sheet.tex`，点击界面上的绿色箭头开始编译。

    在下方窗口可看到 TeXstudio 使用的编译命令为：`xelatex -synctex=1 -interaction=nonstopmode "ACM-cheat-sheet".tex`

1. 懒人版镜像。如果不想进行上述繁琐安装，可使用已配置好的 Ubuntu VMware 虚拟机镜像（已安装 TeX Live 2013、TeXstudio 和字体；详细安装日志见压缩包注释），下载地址：[pan.baidu.com/s/1eQEFLHw](http://pan.baidu.com/s/1eQEFLHw)。

## 如何贡献代码
编译通过后，即具备完整的 LaTeX 编译环境。

本书模板已写好，基本不需要很多 LaTeX 知识即可动手。

欢迎为本书添加内容或纠正错误。在本地编译成 PDF，预览无误后，提交 Pull Request 即可。

## 北美求职微博群
我和我的小伙伴们在这里：[q.weibo.com/1312378](http://q.weibo.com/1312378)
