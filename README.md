c3crmpanel
==========

<a href="http://www.c3crm.com" target="_blank">易客CRM</a>运行环境专用控制面板介绍<br>
<img src="http://www.c3crm.com/d/file/fwzx/cjwt/2013-03-14/fec746c2e8701ad80958b9ad53c8ee7e.jpg"><br>
易客CRM控制面板是采用快手和AAuto编程语言开发，针对xampp运行环境开发的控制面板，功能介绍如下：<br>
1、服务启动apache和mysql,自动修改路径参数<br>
复制"CRM.exe"文件到xampp文件夹下，双击运行，系统自动修改相关配置文件的路径和判断所在的目录是否正确。例如，易客CRM系统默认安装在d:\xampp目录下，现在如果您想把易客CRM安装在c盘 或者e盘，复制xampp目录到硬盘根目录下，然后把CRM.exe复制xampp文件夹下，并双击运行，控制面板就会自动修改相关的系统路径文件，无需手动修改配置文件，易客CRM就可以在c盘或e盘正常运行了。在弹出的控制面板上启动apache和mysql运行环境即可，启动后，apache和mysql将开机后自动启动，CRM.exe也将开机自动启动。也可以根据需要选择不同的端口启动apache和mysql<br>
注意：易客CRM一定要装在xampp目录下，目录名字必须是xampp目录，而且xampp目录必须放在硬盘的根目录下，例如d:/xampp，c:/xampp和e:/xampp等目录。如果不对，系统将提示错误。<br>
2、任务计划<br>
任务计划可以设置每隔一段时间自动通过http访问htdocs下的某个文件，以自动发邮件为例：<br>
易客CRM后台发送邮件的文件是 D:/xampp/htdocs/dosedmail.php，通过http://localhost/dosendmail.php可以发送邮件，那么在任务计划里只需要添加dosendmail.php即可，不管是启动的是80端口还是88端口都可以正常运行。<br>
3、备份还原<br>
根据设置的数据库用户信息，系统会按照设置的时间每天自动备份数据库和htdocs目录下的文件。也可以通过备份的文件自动还原系统。<br>
4、ftp远程备份<br>
如果有设置ftp账号信息，系统还可以把备份的文件上传到远程ftp服务器上，ftp服务器自动保存最新7日内的数据，7日前的数据将自动删除。<br>