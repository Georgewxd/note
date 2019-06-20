# 一、what asp？
ASP，它的原文是 Active Server Pages 。
ASP最核心的扩展内容：ActiveX组件。
# 二、本地搭建小型asp服务器
1.使用软件：小旋风asp、aspsever等
2.搭建步骤：
![](https://picsbed-1256391073.cos.ap-beijing.myqcloud.com/blog20190620191959.png)
下载软件
![](https://picsbed-1256391073.cos.ap-beijing.myqcloud.com/20190620192702.png)
下载asp源码
![](https://picsbed-1256391073.cos.ap-beijing.myqcloud.com/20190620192824.png)
选择端口、根目录及主页
*****
启动asp服务器，本地访问即可
![](https://picsbed-1256391073.cos.ap-beijing.myqcloud.com/20190620193024.png)

# 三、IIS搭建asp服务器
1.选用的环境是win sever 2003
2.开始-->管理您的服务器-->添加或删除角色-->下一步-->选中应用程序服务器-->下一步完成。
![](https://picsbed-1256391073.cos.ap-beijing.myqcloud.com/20190620193725.png)
![](https://picsbed-1256391073.cos.ap-beijing.myqcloud.com/20190620193837.png)
3.创建完成进入IIS管理器，右击网站，新建网站
![](https://picsbed-1256391073.cos.ap-beijing.myqcloud.com/20190620194059.png)
4.网站描述:网站名-->网站ip地址即本机地址，端口默认80，主机头与ip地址相同
![](https://picsbed-1256391073.cos.ap-beijing.myqcloud.com/20190620194350.png)
5.选择网站路径，即网站根目录（网站源码目录）
![](https://picsbed-1256391073.cos.ap-beijing.myqcloud.com/20190620194500.png)
6.勾选如图选项，完成即可。
7.接下来可用ip地址进行访问
*****
### 可能出现的问题
1.Directory Listing Denied
This Virtual Directory does not allow contents to be listed.
问题原因：未将主页添加到默认内容文档中
![](https://picsbed-1256391073.cos.ap-beijing.myqcloud.com/20190620194948.png)
解决方法：邮寄网站，属性，文档-->创建网站默认主页名
![](https://picsbed-1256391073.cos.ap-beijing.myqcloud.com/20190620195147.png)
2.无法找到该页
您正在搜索的页面可能已经删除、更名或暂时不可用。
![](https://picsbed-1256391073.cos.ap-beijing.myqcloud.com/20190620195250.png)
解决办法：web服务扩展中启用ASP
![](https://picsbed-1256391073.cos.ap-beijing.myqcloud.com/20190620195415.png)
