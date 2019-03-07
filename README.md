***READ FIRST***

* If you want to run this program, you need to work around this, run regedit.exe, and navigate to
* 如果你要运行此程序，需要运行regedit.exe，然后找到如下键：
```
    HKEY_CLASSES_ROOT\TypeLib\{0EA692EE-BB50-4E3C-AEF0-356D91732725}
```
* There should only be one subfolder in this class called 1.1. If you see 1.0 or any other folders, you'll need to delete them. Each time after Windows updated or office updated,folder 1.0 will be added.The final hierarchy should look like this:
* 在此键下应该只出现一个子键 1.1，如果你发现有子键1.0，请删除掉，否则程序将不能运行。一般Windows或Office更新后都会添加子键1.0,如果你发现软件运行不了，请按此方法删除掉子键1.0即可。删除后最后的层级应该看起来和如下图示类似。
```
    |- {0EA692EE-BB50-4E3C-AEF0-356D91732725}
    |     |- 1.1
    |         |-0
    |         | |- win32
    |         |- FLAGDS
    |         |- HELPDIR
```

***DOWNLOAD AND INSTALLATION***

* You will find a zipped file named with onetoolXXXX.rar, download this file and unzip it on your own computer. Find the onetool.exe file and double click to run it.
* 你将发现一个名为onetoolXXXX.rar的压缩文件，下载此文件到你的电脑，解压缩，找到onetool.exe文件，然后双击运行它。

### 1，WHAT IS THIS FOR？此程序的用途

* It's a small tool which import text file(s) , web page(s) to Microsoft OneNote software，even can directly import a complete epub format book to OneNote.
* 可以用此程序把文本文件，网页文件批次性的导入到微软的OneNote软件中，甚至可以把ePub书籍直接完整的导入到OneNote中

### 2，WHAT DO WE NEED TO DO FOR DOCUMENT？我们需要对文件做什么？

* For single text file, it treats it as a book. This text file should be formatted as below, chapter title is in a separate line without whitespace at start, and each paragraph has at least one space indent, otherwise all file will be in one page. Between chapter title and its first paragraph should have no empty line, but between title and last paragraph of previous chapter can have empty line. Finally, title will be put on title area of OneNote page and content will be put on content area.
* 对单一的文本文件，我们当它是一本书，此文本需要做以下格式化，章节标题在独自一行且不能以空格开头，文章的段落开头必须有至少一个空格的缩进，否则整个文本将或作为一个页面对待。章节标题和它的段落之间不能有空行，但和前一章节的段落之间有空行无所谓。最后，章节标题将放置在OneNote的标题栏中，内容放在在OneNote的内容栏中。

**Text 文本**

![Single Text](https://github.com/imloafer/OneTool-exe-/raw/master/images/screenshot0.png)

**Show in OneNote OneNote中显示**

![Show in OneNote](https://github.com/imloafer/OneTool-exe-/raw/master/images/screenshot9.png)
* If one book was cut to many files by chapter,you can load all text files once a time, the first line of file will be title and remaining takes as content. It doesn't care whitespace or empty line.
* 如果一本书被按章节分割为很多文本文件，你可以一次性导入所有文件，每个文件的第一行将作为标题，其余的作为内容。可以不管空格和空行。
* For web pages, such as which unzipped from epub format ebook，or saved web page. It can load all files once a time, the first title of web page will be set to OneNote page title, remaining will set to page content. Also you can split each page to pages by subtitles.
* 对于网页文件,比如epub中解压出来的网页或保存的网页，可以一次性导入到OneNote中，网页的第一个标题将放置在OneNote的标题栏中，剩下的放置在内容栏中。你也可以根据副标题把一个网页分割成几个页面然后分别导入到OneNote中。
* For epub format ebook, it was imported exactly as original epub, and chapter by chapter as below:
* 对于ePub格式书籍，它按照原来的ePub的格式原样的导入到OneNote中。

![epub](https://github.com/imloafer/OneTool-exe-/raw/master/images/screenshot7.png)

### 3，SYSTEM AND SOFTWARE REQUIREMENTS 系统和软件要求

* Windows 10  64 system with OneNote 2016 installed. Technically Windows 7 64 system with OneNote 2016 installed should be ok, also OneNote 2013, OneNote 2019 should be workable.
* Windows 10 64位系统，安装OneNote 2016. 理论上Windows 7 64位系统，安装有OneNote 2016 应该也是可以的，还有OneNote 2013, OneNote 2019应该都是可以工作的。


### 4，CONTACT AND DISCUSSION 联络和讨论
* If you found any bug(s) or need any help, you can post here or send email by imloafer@163.com or join QQ group 635390901.
* 如果你发现任何bug或需要帮助,可以发布在这里，或发送邮件到imloafer@163.com 或加入QQ群635390901.

### 5，DONATION 捐助
+ This software is definately free with full function, if you are willing to give author any donation as motivation it is very appreciated. You can find donation method from ABOUT menu's DONATE submenu. Shown as below:
*  可以免费使用此软件的完整功能，如果你愿意给作者任意捐助作为激励将是非常感谢的。可以在软件的关于菜单中的捐助子菜单中找到捐助方法。如下图所示：

![Donate](https://github.com/imloafer/OneTool-exe-/raw/master/images/donate.png)

### 6, SCREENSHOTS AND DEMONSTRATION 截屏和演示
* Program demonstration
* 程序演示

![Start on](https://github.com/imloafer/OneTool-exe-/raw/master/images/demo.gif)

* setup page
* 设置页面

![setup page](https://github.com/imloafer/OneTool-exe-/raw/master/images/setup_01.png)

* Open epub file
* 打开ePub文件

![Opening File](https://github.com/imloafer/OneTool-exe-/raw/master/images/screenshot3.png)

* Ready to transfer
* 准备发送

![Rready](https://github.com/imloafer/OneTool-exe-/raw/master/images/screenshot4.png)

* Transferring
* 发送中

![On Processing](https://github.com/imloafer/OneTool-exe-/raw/master/images/screenshot5.png)

* Done
* 完成

![Done](https://github.com/imloafer/OneTool-exe-/raw/master/images/screenshot6.png)

* Original epub
* 源ePub中显示

![Original epub](https://github.com/imloafer/OneTool-exe-/raw/master/images/screenshot2.png)

* Show in OneNote
* OneNote中显示

![In OneNote](https://github.com/imloafer/OneTool-exe-/raw/master/images/screenshot8.png)
