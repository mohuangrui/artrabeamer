# artrabeamer
## A Beamer template for easily positioning and manipulating content

<h1 align="center">
<img width="100%" src="https://github.com/mohuangrui/mohuangrui/blob/main/gallery/artrabeamer_english.gif" alt="Beamer English">
<img width="100%" src="https://github.com/mohuangrui/mohuangrui/blob/main/gallery/artrabeamer_chinese.gif" alt="Beamer Chinese">
</h1>

## Compilation: requires LaTeX environment
* Just compile like an ordinary Beamer/LaTeX: `pdflatex+biber+pdflatex+pdflatex`
* Switch to Chinese: just add the "CJK" option in "artrabeamer.tex"
```Tex
\usepackage[CJK,biber,authoryear,tikz,table,xlink]{Style/artrabeamer}}
```
* Many other functionalities: check the available options in "artrabeamer.tex" below the line
```Tex
\usepackage[biber,authoryear,tikz,table,xlink]{Style/artrabeamer}
```

## Useful commands added to generic LaTeX
```Tex
\enorcn{English}{Chinese}: automatically switch between English and Chinese versions
\tikzart[t=m]{}}: draw coordinate system to help you position contents
\tikzart[t=p,x=-7,y=3,w=4]"comments"{figname}}: position a picture named "figname" at location "(x,y)" with width "w=4" and comments below the picture.
\tikzart[t=o,x=0,y=-0.8,s=0.8]{objects-such-as-tikz-diagrams}}: position objects at location "(x,y)" with scaling "s=0.8"
\tikzart[t=v,x=9.5,y=-6.5,w=0.5]{Video/vortex_preserve_geo.mp4}[\includegraphics{cover_image}]}: position a video at location "(x,y)" with a cover image of width "w=0.5"
\lolt{lowlight}}, \hilt{highlight}: make the item show in different color when in different state
```

# artrabeamer
## 可轻松安置和操纵内容的Beamer模板

## 编译: 需要 LaTeX 编译环境
* 正常编译即可: `pdflatex+biber+pdflatex+pdflatex`
* 编译生成中文版本：只需在"artrabeamer.tex"中加上"CJK"选项: 
```Tex
\usepackage[CJK,biber,authoryear,tikz,table,xlink]{Style/artrabeamer}}
```
* 从中文版本切换为英文版本：只需在"artrabeamer.tex"中移除"CJK"选项: 
```Tex
\usepackage[biber,authoryear,tikz,table,xlink]{Style/artrabeamer}}
```
同时删除旧的`Tmp`文件夹中的编译缓存文件。

* 更多功能：查看"artrabeamer.tex"文件中的位于如下行下面的诸多选项
```Tex
\usepackage[biber,authoryear,tikz,table,xlink]{Style/artrabeamer}
```
## 新增的有用命令
```Tex
\enorcn{English}{中文}: 自动切换中英文文本
\tikzart[t=m]{}}: 绘制坐标系以帮助定位内容
\tikzart[t=p,x=-7,y=3,w=4]"comments"{figname}}: 将一张名为“figname”的图片放置在位置（x，y）处，图片宽度为“w=4”，并在图片下方添加注释。
\tikzart[t=o,x=0,y=-0.8,s=0.8]{objects-such-as-tikz-diagrams}}: 将对象定位在位置（x，y）处，缩放比例为“s=0.8”
\tikzart[t=v,x=9.5,y=-6.5,w=0.5]{Video/vortex_preserve_geo.mp4}[\includegraphics{cover_image}]}: 将视频放置在位置（x，y）处，封面图像宽度为“w=0.5”
\lolt{lowlight}}, \hilt{highlight}: 低亮/高亮文本
```
