# 最新版本：v1.2.3 #
升级前请阅读下方的更新日志。

从v1.0.x升级请参考Wiki：[如何从v1.0.x升级到v1.1.0](https://github.com/shifujun/UESTCthesis/wiki/%E5%A6%82%E4%BD%95%E4%BB%8Ev1.0.x%E5%8D%87%E7%BA%A7%E5%88%B0v1.1.0)
# 简介 #
UESTCthesis是电子科技大学毕业论文官方发布的LaTeX模板。同时支持本科、各种硕士、各种博士的学位论文排版。
这个模板可以仅使用一条\documentclass命令，就能帮助排版你的毕业论文。
所有文件都使用 UTF-8 无 BOM 编码格式。

本模板使用LPPL协议发布。

模板的**使用说明**请看Wiki页面：  
[https://github.com/shifujun/UESTCthesis/wiki](https://github.com/shifujun/UESTCthesis/wiki)

模板的已知但未能修复的BUG见issue页面：  
[https://github.com/shifujun/UESTCthesis/issues](https://github.com/shifujun/UESTCthesis/issues)

如果有需要反馈的问题可以开issue在这里反馈，我能及时收到邮件。

如果希望用QQ即时交流可加QQ群：   
![成电LaTeX技术交流（71480604）](https://github.com/shifujun/UESTCthesis/wiki/images/QQGroupLogo.jpg) 成电LaTeX技术交流（71480604）验证信息请说明身份，不要空置。  
加群连接：[http://url.cn/S1QIdM](http://url.cn/S1QIdM)

# 更新日志 #
## 2015年5月28日： v1.2.3 ##
- 修复由于ctex宏包更新到2.0.2所带来的兼容性问题。
- 参考文献bst文件中设置的参考文献标题首字母大写已取消。想设置的同学自行参考wiki修改。
- 修复bachelor选项下不能使用english的问题。但english选项本就是给留学生准备的，这样使用并无规范可参考。此更新只是使这两个选项可以正常编译。

## 2015年4月23日： v1.2.2 ##
- 修正参考文献的悬挂缩进不对齐的问题。
- 自动将参考文献条目的标题改为只有第一个字母大写。

## 2015年4月19日 ##
- Fix [issue #39](https://github.com/shifujun/UESTCthesis/issues/39).范例和Wiki中的电子文献类型错写为standard了。应为digital。只修改了Wiki和范例的bib文件。模板的cls和bst未更改，故不更新版本号。
 
##2015年4月10日： v1.2.1  ##
- 修复公式前后段距未能生效的问题。
- 改正致谢页眉有空格的问题。
- 校正页眉、页眉线、版心与页眉间距。
- 设置所有五号字的行距为固定的20磅。
- 修正子图环境的子图标题超过一行时与主标题间距不对的问题。
- 修正章节标题的段前段后距离，以及3级节标题在页首时段前间距没有取消的问题。
- 修正节标题序号没有加粗的问题。
- 修正章节标题序号与题目之间的空格，改为固定的0.5em宽。
- 修正图表公式序号中间的连字符为普通的减号，以便和MS Word一致。

##2015年4月8日： v1.2.0  ##
- 大幅修改bst参考文献格式控制文件。更新后的模板可以生成和规范相同的参考文献格式。但不再支持GB/T7714-2005，也不兼容之前的bib文件。基本上之前定义的参考文献条目都需要进行类型的更改和字段的补全。详情请看Wiki:[录入参考文献和研究成果](https://github.com/shifujun/UESTCthesis/wiki/%E5%BD%95%E5%85%A5%E5%8F%82%E8%80%83%E6%96%87%E7%8C%AE%E5%92%8C%E7%A0%94%E7%A9%B6%E6%88%90%E6%9E%9C)。

##2015年3月25日： v1.1.2  ##
- 对照研究生院新的Word范例调整段距，包括章节标题和图表标题以及图表的前后段距。

## 2015年3月10日 ##
- 修正cv选项使用的cv.tex没有设置页眉。因不涉及cls文件故版本号不变。使用cv选项出现页眉错误的用户单独下载这个文件即可。

##2015年3月3日： v1.1.1  ##
- 修正BUG：缩略词表中的英文全称显示为缩写形式。

##2015年2月13日： v1.1.0 ##

- 去除封面、中文扉页、英文扉页、版权页等前置页面。新解决方案：[添加封面并准备提交电子档](https://github.com/shifujun/UESTCthesis/wiki/%E6%B7%BB%E5%8A%A0%E5%B0%81%E9%9D%A2%E5%B9%B6%E5%87%86%E5%A4%87%E6%8F%90%E4%BA%A4%E7%94%B5%E5%AD%90%E6%A1%A3 "添加封面并准备提交电子档")；
- 删除withoutforepages选项；
- 在onlychapters选项中去除个人和学校信息；
- 新增子图组跨页命令`\subpicnewpage`，用法见Wiki：[子图组跨页](https://github.com/shifujun/UESTCthesis/wiki/%E6%8F%92%E5%85%A5%E5%9B%BE%E7%89%87#%E5%AD%90%E5%9B%BE%E7%BB%84%E8%B7%A8%E9%A1%B5 "子图组跨页")；
- 新增了5个图表命令，用于插入图表时单独设置它们在图表目录中的标题。用法见Wiki：[令图表目录中的标题和正文中不同](https://github.com/shifujun/UESTCthesis/wiki/%E5%9B%BE%E8%A1%A8%E7%9B%AE%E5%BD%95#%E4%BB%A4%E5%9B%BE%E8%A1%A8%E7%9B%AE%E5%BD%95%E4%B8%AD%E7%9A%84%E6%A0%87%E9%A2%98%E5%92%8C%E6%AD%A3%E6%96%87%E4%B8%AD%E4%B8%8D%E5%90%8C "令图表目录中的标题和正文中不同")；
- 删除了pdf元信息中的版权连接，因该链接已失效；
- 删除图表目录中每章条目之间的空白。恢复方式见Wiki：[按章分组](https://github.com/shifujun/UESTCthesis/wiki/%E5%9B%BE%E8%A1%A8%E7%9B%AE%E5%BD%95#%E6%8C%89%E7%AB%A0%E5%88%86%E7%BB%84 "按章分组")；
- 重构了cls文件中主要符号表和缩略词表的实现代码，方便用户修改。修改方式见Wiki：[修改格式](https://github.com/shifujun/UESTCthesis/wiki/%E4%BD%BF%E7%94%A8%E4%B8%BB%E8%A6%81%E7%AC%A6%E5%8F%B7%E8%A1%A8%E5%92%8C%E7%BC%A9%E7%95%A5%E8%AF%8D%E8%A1%A8#%E4%BF%AE%E6%94%B9%E6%A0%BC%E5%BC%8F "修改格式")；
- 删除主要符号表和缩略词表中按首字母分组具有的分组间距。恢复方式见Wiki：[恢复分组间距](https://github.com/shifujun/UESTCthesis/wiki/%E4%BD%BF%E7%94%A8%E4%B8%BB%E8%A6%81%E7%AC%A6%E5%8F%B7%E8%A1%A8%E5%92%8C%E7%BC%A9%E7%95%A5%E8%AF%8D%E8%A1%A8#%E6%81%A2%E5%A4%8D%E5%88%86%E7%BB%84%E9%97%B4%E8%B7%9D "恢复分组间距")；
- 删除了嵌套的枚举环境中第2、3、4级的额外标签后间距。
- fix bug：目录页眉中“目录”间应无空格；
- fix bug：english选项下目录标题、子图环境标题标签“图”字、图表目录页眉是中文的问题；
- fix issue #31：clean.sh脚本里需要删除*.glsdefs文件;
- 在clean脚本中保留了log文件，方便查错。

## 2014年3月12日：v1.0.1 ##

- 将数学公式中的字体改回CM字体。此前v0.6.8中有所疏忽，只将特殊符号改回。现在数学公式字体应该和大多数会议论文中的字体一致了。

## 2014年3月12日：v1.0.0 ##

- 因研究生院正式推荐使用本模板，故将版本号改为v1.0.0。可称为正式版了。
- 本版本除版本号外，和v0.6.9完全一致。

## 2014年3月8日：v0.6.9 - 2013年1月14日：v0.2##
见`example`范例中的更新日志一章。

## 源代码更新日志 ##
模板使用dtx编写方式，在source目录中可以编译出模板的源代码文档。其中也有更新日志，包括一些程序内部方面的改动日志。