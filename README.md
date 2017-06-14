# Kotori-Project

### 写在前面

>我决定又开坑了（喂），这次是一个图床（啪）……    
>写这个的原因是没有一个好用的图床啊……不要跟我提新浪的……github那种方法还是饶了我把……    
>好图床应该具有以下几个特点：    
>* 上传图简单，github上传很麻烦，新浪还好，但是需要一个小号才能发出，忘了说最重要的一点，就是后者不能发R18，而且会打上莫名奇妙的水印，这是一个好图床不具备的，至于那些在墙外的google等等，就更谈不上竞争力了    
>* 有权限控制，最开始觉得这些都是很麻烦的，借鉴一下匿名版的思想，传图是无需注册或者说是匿名的，但是可以增加黑名单和，让某些IP无法传图（喂），也可以增加需要登录的部分，登录之后能传不让大家看的图（喂），至于图是什么内容可以发挥你的想象力    
>* 稳定，稳定才是王道，不能像某些免费图床一样，今天能用，明天就跪了；前面也说到g+的相册，但是保不好哪天就被墙了（或者已经被墙了233），另外能支持cdn当然最好，但是我不会配置cdn啊~   
 
>kotori当然是小鸟的意思啦~图床写好之后我马上粘个图片到这儿    
>[图片预留位置]    

### 准备实现功能

>其实[tmp.is](http://tmp.is)这个站已经很接近我的想法了，可惜作者好像不知道干啥去了，现在处于传不上图片的状态233    

* 匿名传图，初步支持jpg, png, webp（看起来要php5.5以上，不过应该都没有用5.3或者5.2的吧）, gif（gif压缩这个php的GD库还是有只会留取1帧的问题待解决）
* 支持登录传图，支持更大的图（好像没什么用），支持不显示在略缩图中（你懂的），还有就是匿名用户是看不到的图（喂）

### 功能划分
>先写个php版本吧（后续的之后再说），看向kagari匿名版    
>完全是静态文件的玩意，用不用数据库呢（试着不用一次试试    

* `index.php` 入口文件
* `lib\Image.php` 图片类Image
* `lib\User.php` 用户类User
* `config\conf.php` 配置文件
* `upload\` 图文件目录
* `thumbs\` 缓存图目录
* `data\userdata` 用户数据
* `data\imagedata` 图片数据


