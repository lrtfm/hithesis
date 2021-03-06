# hithesis
# 哈尔滨工业大学LaTeX论文模板

<a rel="license" href="http://creativecommons.org/licenses/by-nc/4.0/"><img alt="知识共享许可协议" style="border-width:0" src="https://i.creativecommons.org/l/by-nc/4.0/88x31.png" /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" href="http://purl.org/dc/dcmitype/Text" property="dct:title" rel="dct:type">hithesis</span> 由 <a xmlns:cc="http://creativecommons.org/ns#" href="https://github.com/dustincys/hithesis" property="cc:attributionName" rel="cc:attributionURL">https://github.com/dustincys/hithesis</a> 采用 <a rel="license" href="http://creativecommons.org/licenses/by-nc/4.0/">知识共享 署名-非商业性使用 4.0 国际 许可协议</a>进行许可。<br />基于<a xmlns:dct="http://purl.org/dc/terms/" href="https://github.com/dustincys/hithesis" rel="dct:source">https://github.com/dustincys/hithesis</a>上的作品创作。

## What's hithesis?

hithesis is a LaTeX thesis template package for Harbin Institute of Technolog
supporting bachelor, master, doctor dissertations. Since the users of this
package are supposed to be Chinese or those understand Chinese, the following of
this file and all other documents are written in Chinese only.

This file may be distributed and/or modified under the
conditions of the LaTeX Project Public License, either version 1.3a
of this license or (at your option) any later version.
The latest version of this license is in:

http://www.latex-project.org/lppl.txt

and version 1.3a or later is part of all distributions of LaTeX
version 2004/10/01 or later.


## hithesis是什么？

hithesis
旨在建立一个简单易用的哈尔滨工业大学学位论文LaTeX模板，包括本科论文、硕士论文、博士论文
。现 在支持本科、硕士、博士论文，对其它格式的支持会陆续加入。
hithesis 已收录在[CTAN](https://ctan.org/pkg/hithesis
"CTAN")中，用户安装TeXLive将自带我工模板（版本日期>2017.08.28）。

## 我工规范有歧义之处

各位刀客一定要先看清楚我工规范两大歧义之处：[版芯歧义](http://yanshuo.name/cn/2017/06/hithesisregulation/)和[本科生行距歧义](http://yanshuo.name/cn/2017/06/hithesissiyuan/)。

另外注意一处小歧义：在[规范](http://hitgs.hit.edu.cn/aa/fd/c3425a109309/page.htm)中规定和[研究生word排版范例](http://hitgs.hit.edu.cn/ab/1f/c3425a109343/page.htm)的中文目录中出现的“ABSTRACT”和“Abstract”的写法歧义（规格严格功夫大家！！！）。

## 模板特点

### 呆萌的操作，傲娇的效果

- 极限程度实现了[《哈尔滨工业大学研究生学位论文撰写规范》](http://hitgs.hit.edu.cn/aa/fd/c3425a109309/page.htm)、[《哈尔滨工业大学本科生毕业论文撰写规范》](http://jwc.hit.edu.cn/2566/list.htm)
- 这是[PlutoThesis](https://github.com/dustincys/PlutoThesis "PlutoThesis")的终极进化，PlutoThesis废弃不再维护。
 - 更傻更简单的选项，例如论文主文件，只需要在文档类的括号中填写本硕博选项，字体选项（设置弹性间距或者刚性间距），文科生选项（目录可以设成四级目录），非全日制类型等，轻松设定目标格式。
 - 自适应格式，例如图题和标题，标题字号在字数超过两行时自动由五号变小五号，实现自适应（硕博规范规定，字数多时用五号）
 - 自动化中英文索引（博士规范要求，有需要时候添加）
 - 图书馆提交论文级的书签设置
 - ……


### 矫正PlutoThesis的不足

 - 纠正PlutoThesis页面向下溢出
 - 纠正PlutoThesis不符合规范要求的各层次题序及标题不得置于页面的最后两行，改为不得置于最后一行（孤行），从此解决了饱受诟病的空白大的问题。
 - 纠正PlutoThesis行间距与标题段前段后距离统统设置为1.6倍行距的问题
 - 更强大的版芯设置，满足所有需求
 - 补充了PlutoThesis没有的符号表、索引两项
 - 字体设置符合CTeX的自动识别系统功能
 - 纠正PlutoThesis中图片中一些距离设置
 - 添加了符合规范要求的“图注在图题之上的设置”
 - 纠正PlutoThesis的双语图、表题中英语的非两端对齐问题
 - 添加了PlutoThesis中没有的图题最后一行居中且两端对齐格式
 - 添加了所有的图形排版格式
 - 纠正了附录中标题错误
 - 纠正了博士论文右翻页问题
 - 添加扫描替换功能，替换之后、页码目录书签自动设置
 - 添加思源宋体设置，再也不用害怕奇怪字打不出来了
 - 添加文科生、非全日制同等学力封面格式
 - 添加PlutoThesis没有的说明文档
 - ……

### 为了我工的规格严格、功夫到家

 - 行间距、段前后距离设置精确到小数后四位， 例如 1bp = 1.00374pt，1mm = 2.84526pt， 按照我工之要求, 行距在3mm～4mm之间，换算之后为20.50398～23.33863bp，严格符合规范要求，哪怕是显微镜级别
 - 规范明确规定，数字间空格要求为汉字宽度的四分之一（形式类似与 12 2345 和 0.123 456 这样多于3位以上的整数或小数）。默认情况下在LaTeX中任何人工输入的空格均不正确（“\:”为4/18汉字宽度，“\;”为5/18汉字宽度，所以PlutoThesis中的数字间宽度错误)。hithesis模板中定义了精准的数字间宽度。
 - 重写了一堆重要函数，例如章节标题由原来的`BiChapter{}{}`方式进化为`chapter{}[]`，极大简化，后面方括号中为可选括号，硕本可以不用，用了自动忽略
 - 严格符合（满足）两个规范要求，由于规范中有矛盾之处，例如本科生的标题段前距离有两处不一样的规定，刚性行距尽量满足行数（要求约33行）要求。
 - 规范中给出了行距区间，为了规格严格，设置了弹性行距
 - ……

## 关于模板的命名和其他说明

### 模板的命名

本模板对PlutoThesis中的核心代码进行了彻底深入的修改。
PlutoThesis中没有采用cls，这种文档类的模式，代码与正文内容耦合程度大难以维护，本科模板和硕博模板难以融合。
由于冥王星已经不是太阳系C9之一，所以不继续使用PlutoThesis命名。

hithesis, 既含我工hit，也是说用的“嗨！”，读作“嗨thesis”。

### 关于模板的下载地址

模板有三个下载地址：

1. github: https://github.com/dustincys/hithesis
2. gitee: https://gitee.com/dustincys/hithesis
3. CTAN: https://ctan.org/pkg/hithesis

github和gitee的版本是同步且是最新的模板。
CTAN的版本一般会比较落后，但在每年年底会同步为最新版本。

### 关于hithesis的线上讨论区

由于维护者（就是本书呆）已经是高龄不毕业刀客，课题繁忙，常常无法及时回答疑问。
为了解决使用中遇到的问题，请各位刀客和大侠加入QQ群：259959600。
群里有很多热心的LaTeX隐士高人如@poofee等，很乐于解答。

### 关于查重

注意：我工的论文查重可以使用pdf查重！！！！！！！

另外一点注意：查重的pdf一定要确保能够正常复制汉字。有些系统自动识别的汉字字体，
会出现无法正常复制的情况（可能是系统的字体映射出现了误差）。一般需要在主文件的
选项中明确声明使用哪一种fontset。

### 模板的编译方法、打印版、电子版及其他说明

- 生成论文格式文件(第一步要生成 *.cls，*.cfg，*.ist，然后再生成论文)

		latex hithesis.ins

- 生成论文

		xelatex main.tex
		bibtex main
		xelatex main.tex
		xelatex main.tex
		splitindex main -- -s hithesis.ist  # 自动生成索引
		xelatex main.tex

- 生成文档

		xelatex hithesis.dtx
		makeindex -s gind.ist -o hithesis.ind hithesis.idx
		makeindex -s gglo.ist -o hithesis.gls hithesis.glo
		xelatex hithesis.dtx
		xelatex hithesis.dtx

如果喜欢Makefile的是另一画风：

- 生成文档类

		make cls

- 生成论文

		make thesis

- 生成文档

		make doc

LaTeX 中的ctex package版本要求：

	ctex >= v2.4.3 (2016年9月份发布)

注意，一般情况下，博士论文的打印版要求右翻页，最后向图书管提交的电子版不是右翻
页，注意选项中的选项。

由于维护者（就是本书呆）已经是高龄不毕业博士，课题繁忙，实在无空余时间再写详细文档以及 无偿解决一些用户要求（例如前面文档中[已经解决的算法格式各实验室要求不一致](https://github.com/dustincys/PlutoThesis#%E6%B2%A1%E6%9C%89%E6%98%8E%E7%A1%AE%E8%A6%81%E6%B1%82%E7%9A%84%E6%A0%BC%E5%BC%8F)问题）。

各位刀客和大侠如用的嗨，要解囊相助，请微信扫码～～

![5](http://wx4.sinaimg.cn/large/61dccbaaly1fge32sbb32j20my0uz3zt.jpg "谢谢")

如果用的非常嗨，

![10](http://wx4.sinaimg.cn/large/61dccbaaly1fge32tuvvsj20my0uzabc.jpg "谢谢")

那个，看在苦X高龄不毕业博士，还熬夜写代码的份上…… 唉……

![1](http://wx4.sinaimg.cn/large/61dccbaaly1fge32qrvgij20my0uzjso.jpg "谢谢")

或者支付宝，不限额度，

![zfb](http://wx3.sinaimg.cn/large/61dccbaaly1fizali9tafj20k00ucgos.jpg "谢谢")

其实没关系，为了我工的“规格严格，功夫到家”！

- 本模板以PlutoThesis为核心基础，参考了CTAN中清华大学薛瑞尼所开发的thuthesis以及其分支重庆大学等毕业论文模板的代码开发而来
- ~~学校教务处和研究生院只提供了规范，并没有提供官方的任何模板（包括word），所以~~ 学校教务处和研究生院提供了规范和[研究生word模板](http://hitgs.hit.edu.cn/ab/1f/c3425a109343/page.htm)以及[本科生word模板](http://jwc.hit.edu.cn/2566/list.htm)(厉害了word哥……)，此模板仅为规范的参考实现，不保证格式审查老师不提意见。任何由于使用本模板而引起的论文格式审查问题均与本模板作者无关

<a rel="license" href="http://creativecommons.org/licenses/by-nc/4.0/"><img alt="知识共享许可协议" style="border-width:0" src="https://i.creativecommons.org/l/by-nc/4.0/88x31.png" /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" href="http://purl.org/dc/dcmitype/Text" property="dct:title" rel="dct:type">hithesis</span> 由 <a xmlns:cc="http://creativecommons.org/ns#" href="https://github.com/dustincys/hithesis" property="cc:attributionName" rel="cc:attributionURL">https://github.com/dustincys/hithesis</a> 采用 <a rel="license" href="http://creativecommons.org/licenses/by-nc/4.0/">知识共享 署名-非商业性使用 4.0 国际 许可协议</a>进行许可。<br />基于<a xmlns:dct="http://purl.org/dc/terms/" href="https://github.com/dustincys/hithesis" rel="dct:source">https://github.com/dustincys/hithesis</a>上的作品创作。
