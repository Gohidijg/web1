# web1

 archlinux中文乱码解决
 
pacman -S wqy-zenhei ttf-fireflysung(flash乱码) 
 
/etc/locale.gen 设置en_US.UTF8 UTF-8 zh_CN.UTF8 UTF-8 
 
locale-gen   www.myhack58.com  
 
locale 
 
locale -a 
 
/etc/rc.conf 中 
 
LOCALE=en_US.UTF-8 
 
在google浏览器中设置中文字体

-------------------------------------------------------------------

fonts-chinese-3.02-12.el5.noarch.rpm

   fonts-ISO8859-2-75dpi-1.0-17.1.noarch.rpm

   没有的话，就到网上去下，找好之后，打开终端，执行这两句命令：

    rpm -ihv fonts-chinese-3.02-12.el5.noarch.rpm

    rpm -ihv fonts-ISO8859-2-75dpi-1.0-17.1.noarch.rpm

    安装好之后，还得设置下：

    vi /etc/sysconfig/i18n

     修改为：

    LANG="zh_CN.GB18030"
    LANGUAGE="zh_CN.GB18030:zh_CN.GB2312:zh_CN"
    SUPPORTED="zh_CN.GB18030:zh_CN:zh:en_US.UTF-8:en_US:en"
    SYSFONT="lat0-sun16"
    
    -----------------------------------------------------------------
    
    
    
