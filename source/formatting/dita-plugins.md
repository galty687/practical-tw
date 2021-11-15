# DITA Plugins

在开发DITA样式的时候，一个比较好的实践就是把不同样式制作为插件，例如用户手册插件，参考手册插件，WebHelp插件等。这样在使用的时候比较方便，例如可以让你的同事使用你的样式发布，不需要额外配置，plugin中有全部所需的内容。

## 实例

oXygem XML 将他们公司的手册的样式作为插件分享出来了，我们可以尝试安装他们的样式插件，并用于发布自己的内容。

步骤：
1. 下载 [oXygen XML 插件](https://github.com/oxygenxml/com.oxygenxml.pdf2.ug)
2. 安装插件 
  

   
    `dita install com.oxygenxml.pdf2.ug-master.zip`
   

   
    提示：Added com.oxygenxml.pdf2.ug            
   
3. 使用该插件发布内容。格式为（oxy-ug-pdf）
    
    `dita --input=projector_user_manual.ditamap --format=oxy-ug-pdf`
   
    
     提示：需要定义中文字体，否则会出现乱码





