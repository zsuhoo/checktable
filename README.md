# checktable

&emsp;&emsp;这个项目主要用来展示调用百度API实现图像文字识别的功能，利用该工具在某些情况下可以快速核对纸质版与电子版信息之间的差异，得到高效工作的目的。


&emsp;&emsp;打包成可运行jar包，如果要直接运行，下载checktable_release1.1文件夹，然后看里面的“使用说明.txt”来使用就可以了。

### 软件说明及具体操作
本软件是具有核对纸质版与电子版信息是否一致的功能，利用百度API文字识别的接口。（当前以核对高校教育厅励志奖学金表格为例）

1. 只要修改info.properties配置中的image_path，excel_path，target_path这个三个路径就可以了，路径说明在info.properties有备注。<br/><br/>
2. 修改完info.properties之后保存，如果是用window记事本打开的要选择另存为，然后在保存编码那里选择utf-8.<br/><br/>
3. 然后点击“点击这个运行.bat”这个就可以开始运行了。直到命令行出现请"按任意键继续. . .","已经全部输出到文件中了！"等信息出现，就表示已经识别好 了。这是就可以打开target_path中定义的excel文件，就会出现纸质版的信息了。<br/><br/>
4. 2018年10月3日新增重新识别电子版信息和纸质版信息功能，如果在第三步得到的纸质版信息不准确，可以自己手动修改好，点击“点击这个重新比较电子版信息和纸质版信息.bat”，就能重新比较excel_path，target_path这两个文件的差别，得到新的核对信息，并重新输出到target_path这个文件中。<br/><br/>

### 注意事项：<br/><br/>
1.student_info.txt文件运行就会出现，也是纸质版的识别内容信息，不过只是txt文件。<br/><br/>
2.上面所有使用到的excel表都是2003年的格式即使以xls结尾的表格，不然会出现问题。<br/><br/>
3.在使用excel_path要核对的电子表信息时，要复制本目录下的模板过去，将要核对的内容复制到模板中去（保留第一行，即标题栏）。<br/><br/>
4.要保证image_path中图片的顺序与excel_path表中信息的顺序一致。即第一张图片要对应excel_path表中的第二行数据（因为第一行为标题）。第二张图片要对应excel_path表中的第三行数据。<br/><br/>
5.需要使用jdk1.7及以上的环境运行。<br/><br/>
6.注意 贫困等级很大可能识别错误，需要人工核对。<br/><br/>



### 使用示范动画
<img alt="使用示范动画" src="https://raw.githubusercontent.com/KANLON/checktable/master/img/check-table.gif"/>
<img alt="使用示范动画2" src="https://raw.githubusercontent.com/KANLON/checktable/master/img/check-table.gif"/>



如有问题请联系：<br/>
制作者：zhangcanlong<br/>
联系方式：Canlong2015@126.com<br/>
