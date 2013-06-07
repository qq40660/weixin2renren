weixin2renren
=============

通过微信公众帐号发布消息到人人公共主页/树洞的demo  
  
使用web.py框架  
  
代码中需完善一些应用信息  
  
最开始的token可以在下面链接中获取：(其中的api key 、api secret指的是[人人应用](http:dev.renren.com)的参数）  
https://graph.renren.com/oauth/authorize?client_id=your_api_key&redirect_uri=your_redirect_uri&response_type=code&scope=status_update+photo_upload+admin_page  
https://graph.renren.com/oauth/token?grant_type=authorization_code&client_id=your_api_key&redirect_uri=&client_secret=your_api_secret&code=上面地址授权后获得的code  
  
access_token 有效期好像是一个月左右，过期后代码已设置为自动更新，不过是每次要发消息都要更新，比较没效率。  
所以一旦过期建议手动修改代码中的access_token。  
  
联系： strak47@gmail.com
