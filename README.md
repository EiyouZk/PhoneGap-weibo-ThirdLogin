# PhoneGap-weibo-ThirdLogin





## 问题及解决方法


（1）问题：iOS 报错 sso package or sign error 

     解决：由于ios TARGETS => General => Bundle ID 和微博开放平台所填写的不符合。
     

（2）问题：ios 拉起授权页面之后，还没点确定，直接返回。

     解决：回调结果是ok的，可能上次授权还在有效期之内，不需要重新授权。
     
     
（3）问题：授权webview弹窗立即消失，跳转到微博页面，无法返回猿app登录第三方登陆页面。

     解决：1）、看看info.plist文件里有没添加加url types，在url schems里填上wb+APPKEY，如：wb8728171  

          2）、微博平台上设置的bundle id 是否与你的应用一致
          
          
（4）问题：授权页面无法显示原app的图标。
 
     解决：检查WEIBO_APP_ID是否准确
     
