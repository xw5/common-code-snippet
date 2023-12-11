# 前端开发常用代码段插件
>根据缩写快速提供代码模板，提高开发速度，代码段持续更新中......
<br />

## 使用建议
>考虑到用户的记忆成本，用户无需记忆所有代码段的缩写，输入特殊开头字符则会带出当前类别下的代码段，优化使用体验，定义如下使用规则：
>- 在js/jsx下输入js则会带出所有属于js的代码段
>- 在jsx下输入r则会带出所有属于react的代码段
>- css,less,scss下输入css则会带出所有属于css的代码段
>- html下输入html会带出所有属于html的代码段
>- mardown下输入md会带出所有属于markdown的代码段
>- 全局输入gb(global的缩写)会带出全局的代码段
>- 支持不带特殊符号的输入形式：如cssellipsis和ellipsis都能带出css下单行省略号的代码段
>- 代码段匹配字段都会尽量使用语义化的字段,如mdol:在mardown下输入无序列表;cssarrowtop:css实现的向上箭头，这样可以让用户记忆不再有太大负担
>- 同时部分代码段支持中文关键字，如(js代码段里的深拷贝、事件委托...),详情见下面说明文挡

<br />

## 注意事项
> - markdown等文本输入环境默认是无法开启代码提示和tab自动补全的，如果想要使用代码段则可在vs code中的setting.json加如下配置
>  ``` json
>    "editor.tabCompletion": "on",
>    "[markdown]": {
>        "editor.wordWrap": "on",
>        "editor.quickSuggestions": true
>    }
>  ```
<br />

## 目前支持的模板

### Javascript代码模板

|  缩写  |  模板  
|  ----  |  ----  
|  jsvar  |  js 定义变量代码段 关键字："var", "jsvar"
|  jsfor  |  js for基本用法 关键字: "for","jsfor"
|  jsforof  |  for-of循环 关键字: "forof","jsforof"
|  jsforin  |  for-in循环 关键字: "forin","jsforin"
|  jsif  |  if语句 关键字: "if", "jsif"
|  jselse  |  if下的else语句 关键字: "else", "jselse"
|  jselseif  |  if下的elseif语句 关键字: "elseif", "jselseif"
|  jsswitch  |  js下switch语句 关键字: "switch", "jsswitch"
|  jstry  |  js下try catch语句 关键字: "try","jstry"
|  jsfunction  |  js function定义结构 关键字: "function","jsfunction"
|  jslog  |  js下console.log语句 关键字: "log","jslog"
|  jslog-  |  js下console.log语句,console.log('----test----:', test); 关键字: "log-","jslog-"
|  jsclass  |  js 类定义结构 关键字: "class","jsclass"
|  jspromise  |  js Promise定义结构 关键字: "promise", "jspromise"
|  jsregex  |  常用正则表达式集合(用户名、密码、手机号、邮箱、身份证...) 关键字: "regex", "jsregex"
|  jsthrottle  |  js下节流代码段 关键字: "jsthrottle","throttle","jsjl"
|  jsdebounce  |  js下防抖代码段 关键字: "jsdebounce","debounce","jshd"
|  jsstore  |  vue状态管理主文件模板代码段 关键字: "jsstore","store"
|  jsstoremodule  |  vue状态管理module模板代码段 关键字: "jsstoremodule","storemodule"
|  jsdialogdrag  |  el弹窗拖拽指令 关键字: "jsdialogdrag","dialogdrag","饿了么弹窗拖拽","弹窗拖拽"
|  jsrem   |  移动端rem计算代码段  关键字:  "jsrem", "rem"
|  jsimport   |  import{}语句代码段  关键字: "import", "jsimport"
|  jsimportdefault   |  importdefalt语句代码段 关键字:  "importdefault", "jsimportdefault"
|  jscsfn  |  js const定义箭头函数代码段  关键字: "csfn", "jscsfn","常量函数"
|  js?/js3m  |  js 三目运算代码段 关键字: "js?", "js3m","三目运算"
|  jsArraymethod  |  Array常用方法列表 关键字: "jsarraymethod","arraymethod","jsarray","array"
|  jsStringMethod  |  String常用方法列表 关键字: "jsstringmethod", "stringmethod", "jsstring", "string"
|  jsMathMethod  |  Math对象常用方法 关键字: "jsmathmethod", "mathmethod", "jsmath", "math"
|  jsDateMethod  |  Date常用方法 关键字: "jsdatemethod", "datemethod", "jsdate", "date"
|  jsLocation  |  Location对象属性和方法 关键字: "jslocation", "location"
|  jsHistory  |  History对象方法 关键字: "jshistory", "history"
|  jsDom  |  Dom元素对象 关键字: "jsdom", "dom"
|  jsmobile  |  js判断当前是否在移动端下 关键字: "jsmobile","mobile","判断是移动端","移动端"
|  jsrandom  |  js生成随机范围内的整数 关键字: "jsrandom", "random","区间内随机整数","随机整数"
|  jstype  |  检查JavaScript中任何变量或值的类型 关键字: "jstype", "type","获取数据类型","数据类型"
|  jsurlquery  |  获取url中的query参数 关键字: "jsurlquery", "urlquery","url参数获取"
|  jsadd  |  加法精确计算，避免数据相加小数点后产生多位数和计算精度损失 关键字：jsadd, add, jsnum+,"精确加法","加法"
|  jssub  |  减法精确计算，避免数据相减小数点后产生多位数和计算精度损失 关键字：jssub, sub, jsnum-,"精确减法","减法"
|  jsmulti  |  乘法精确计算，避免数据相乘小数点后产生多位数和计算精度损失 关键字：jsmulti,jsmulti,jsnum*,"精确乘法","乘法"
|  jsdiv  |  除法精确计算，避免数据相除小数点后产生多位数和计算精度损失 关键字：jsdiv, div, jsnum/,"精确除法","除法"
|  jstimeformat  |  时间戳转日期 关键字："jstimeformat", "timeformat","日期格式化"
|  jsurlquerytoobj  |  url参数转对象 关键字: "jsurlquerytoobj", "urlquerytoobj","url参数转对象"
|  jsobjtourlstring  |  对象转化为querystring 关键字: "jsobjtourlstring", "objtourlstring","对象转url参数"
|  jscountdown  |  获取到某一个时间的倒计时对象 关键字: "jscountdown", "countdown", "倒计时"
|  jsleapyear  |  是否闰年 关键字: "jsleapyear", "leapyear", "jsyear", "year","闰年"
|  jsrandomcolor  |  随机生成颜色 关键字: "jsrandomcolor", "randomcolor"
|  jsdatatype  |  数据类型判断 关键字: "jsdatatype", "datatype"
|  jsremoverepeatarray  |  数组去重 关键字: "jsremoverepeatarray", "removerepeatarray","数组去重","去重"
|  jsrandomsortarray  |  数组顺序随机打乱 关键字: "jsrandomsortarray", "randomsortarray","数组随机打乱"
|  jsweixin  |  是否微信内置浏览器，关键字：jsweixin, weixin, jswx, wx
|  jsdaysinmonth  |  获取某个月的天数 关键字: "jsdaysinmonth", "daysinmonth","获取月天数","月天数"
|  jssystemType  |  获取操作系统类型 关键字: "jssystemType", "systemType","获取系统类型","系统类型"
|  jswxapiauthorization  |  微信api授权封装，关键字：jswxapiauthorization, jswx, wx
|  jsaxios  |  简易axios封装，支持重复请求取消 关键字: "jsaxios","axios"
|  jsnumToMillennials  |  数字转千分位 关键字: "jsnumToMillennials", "numToMillennials", "jsnum", "数字转千分位","千分位"
|  jsgetDataType  |  获取数据类型 关键字: "jsgetDataType","getDataType","jsdataType","dataType","获取数据类型","数据类型"
|  jsfullscreen  |  指定元素全屏实现代码 关键字: "jsfullscreen","fullscreen","全屏"
|  jscookie  |  cookie封装(mdn) 关键字: "jscookie","cookie"
|  jslocalstorage  |  localstorage封装,支持设置过期时间 关键字: "jslocalstorage","localstorage","jsstorage","storage","本地存储"
|  jsdeepcopy  |  对象深拷贝 关键字: "jsdeepcopy", "deepcopy", "skb", "深拷贝"
|  jsstoppropagation  |  阻止事件冒泡，兼容ie 关键字: "jsstoppropagation", "stoppropagation", "jsstop", "stop", "阻止冒泡"
|  jspreventdefault  |  阻止事件默认行为，兼容ie 关键字: "jspreventdefault", "preventdefault", "jsstop", "stop", "阻止默认行为"
|  jsgetboundingclientrect  |  阻获取元素位置大小 关键字: "jsgetboundingclientrect", "getboundingclientrect", "jsgetdomrect", "getdomrect", "元素位置大小"
|  jseventdelegation  |  事件委托 关键字: "jseventdelegation","eventdelegation", "事件委托"
|  jsjsonp  |  jsonp请求 关键字: "jsjsonp","jsjsonp"
|  jsajax  |  简易ajax封装 关键字: "jsajax","ajax"
|  jscopy  |  复制文本 关键字: "jscopy","copy","复制"
|  jsgetscrolldistance  |  获取滚动像素 关键字: "jsgetscrolldistance","getscrolldistance","获取滚动像素","滚动像素"
|  jsscrolltotop  |  滚动到顶部 关键字: "jsscrolltotop","scrolltotop","滚动到顶部"
|  jsconvertchineseamount  |  数字转中文大写金额 关键字: "jsconvertchineseamount","convertchineseamount","数字转中文大写金额","中文大写金额"
|  jsisinviewport  |  判断元素是否完全在可视区内 关键字: "jsisinviewport","isinviewport","元素在可视区内","可视区内"
|  jsisintoviewport  |  判断元素是否进入可视区内 关键字: "jsisintoviewport","isintoviewport",,"元素进入可视区内","可视区内"
|  jsintoviewportlistener  |  监听元素进入or离开可视区 关键字: "jsintoviewportlistener","intoviewportlistener","元素进入可视区监听"
|  jsquerySelector  | querySelector选择元素 关键字: "jsqueryselect","queryselect","jsselect","select","元素选择"
|  快速排序  | 快速排序 关键字: "jsquicksort","quicksort","jssort","sort","快速排序","排序"
|  选择排序  | 选择排序 关键字: "jsselectsort","selectsort","jssort","sort","选择排序","排序"
|  插入排序  | 插入排序 关键字: "jsinsertSort","insertSort","jssort","sort","插入排序","排序"
|  冒泡排序  | 冒泡排序 关键字: "jsbubblesort","bubblesort","jssort","sort","冒泡排序","排序"
|  归并排序  | 归并排序 关键字: "jsmergesort","mergesort","jssort","sort","归并排序","排序"
|  桶排序  | 桶排序 关键字: "jsbucketsort","bucketsort","jssort","sort","桶排序","排序"
|  js实现暂停睡眼  | js实现暂停睡眼 关键字: "jssleepsync","sleepsync","jssleep","sleep","暂停","睡眠"
|  获取地理位置  | 获取地理位置 关键字: "jsgetlocation","getlocation","地理位置"
|  H5摇一摇实现  | H5摇一摇实现 关键字: "jsdevicemotion","devicemotion","jsshake","shake","摇一摇"
|  ifplus  |  js代码下专为ifplus-loader定义的条件代码段  关键字: "ifplus","jsifplus"
<br />

### CSS代码段

|  缩写  |  模板  
|  ----  |  ----  
|  cssellipsis  |  单行文本超出省略号 关键字: "cssellipsis", "ellipsis","超出单行省略","单行省略"
|  cssreset  |  css样式重置 关键字: "cssreset", "reset", "样式重置"
|  cssellipsismulti  |  多行文本超出省略号 关键字: "cssellipsismulti","ellipsismulti","超出多行省略","多行省略"
|  csswrap  |  css强制换行 关键字: "csswrap","wrap","文本换行","换行"
|  cssarrowtop  |  css实现朝上箭头 关键字: "arrowtop", "cssarrowtop","上箭头","箭头"
|  cssarrowbottom  |  css实现朝下箭头 关键字: "arrowbottom", "cssarrowbottom","下箭头","箭头"
|  cssarrowleft  |  css实现朝左箭头 关键字: "arrowleft","cssarrowleft","左箭头","箭头"
|  cssarrowright  |  css实现朝右箭头 关键字: "arrowright","cssarrowright","右箭头","箭头"
|  cssgray  |  置灰滤镜 关键字: "gray", "cssgray","置灰滤镜","置灰"
|  cssblur  |  模糊滤镜 关键字: "cssblur", "blur","模糊滤镜","模糊"
|  csscentermargin  |  absolute+margin元素水平垂直居中 关键字: "centermargin","csscentermargin","margin居中","居中"
|  csscentertransform  |  absolute+transform元素水平垂直居中 关键字: "centertransform", "csscentertransform","transform居中","居中"
|  cssplaceholder  |  设置input的placeholder的颜色 关键字: "cssplaceholder", "placeholder"
|  cssmedia  |  media媒体查询参考段 关键字: "cssmedia", "media","媒体查询"
|  cssgradient  |  css渐变参考写法 关键字: "cssgradient", "gradient","渐变"
|  cssnoselect  |  css禁止文本选中 关键字: "cssnoselect", "noselect","禁止选中"
|  cssslectioncolor  |  设置选区背景颜色 关键字: "cssslectioncolor", "slectioncolor","选区颜色"
|  cssflex  |  css flex基本代码 关键字: "cssflex", "flex"
|  cssflexcolumn  |  flex column 关键字: "cssflexcolumn", "flexcolumn"
|  cssflexcenter  |  flex水平垂直居中 关键字: "cssflexcenter", "flexcenter","flex居中","居中"
|  csslink  |  a链接伪类设置顺序 关键字: "csslink", "link"
|  css::border  |  css伪类实现边框 关键字: "css::border", "::border", "伪类border"
|  cssboxshadow  |  css boxshadow盒子阴影 关键字: 
|  csstransition  |  css transition过渡 关键字: "csstransition","transition","缓动动画","动画"
|  csskeyframes  |  css keyframes动画定义 关键字: "csskeyframes","keyframes","帧动画","动画"
|  cssrem  |  css vw+rem适配方案y 关键字: "cssrem", "rem"
|  csshidetext  |  css 用于seo的隐藏文本 关键字: "csshidetext", "hidetext","隐藏文本","seo隐藏文本"
|  cssbackgroundimagefix  |  background-image-size适配样式 关键字: "cssbackgroundimagefix", "backgroundimagefix","背景图片适配"
|  csswh  |  元素宽高设置 关键字: "csswh", "wh"
|  cssmouse  |  css设置鼠标样式 关键字: "cssmouse", "mouse","鼠标"
|  cssevent  |  css实现事件禁止实现元素穿透 关键字: "cssevent", "event","事件穿透","事件"]
|  cssfiletype  |  根据文件格式显示不同的链接样式 关键字: "cssfiletype", "filetype","链接图标"
|  cssmarginauto  |  固定宽度且居中 关键字: "cssmarginauto", "marginauto"
|  cssmask  |  css实现遮罩效果 关键字: "cssmask", "mask","遮罩"
|  cssbackground  |  cssbackground完整写法 关键字: "cssbackground", "background"
|  cssbackgroundimages  |  css实现多背景 关键字: "cssbgimages", "bgimages","多图片背景"
|  cssscrollbarhidden  |  css不显示滚动条 关键字: cssscrollbarhidden, crollbarhidden, scrollbar,"隐藏滚动条"
|  pcfont  |  pc网页推荐设置字体 关键字: pcfont, font,"pc推荐字体","字体"
|  mobilefont  |  移动端网页推荐设置字体 关键字: mobilefont, font,,"移动推荐字体","字体"
|  csslandscape  |  提示用户竖屏浏览 关键字: csslandscape, landscape, csssb, sb,"竖屏提示"
|  cssportrait  |  提示用户横屏浏览 关键字: cssportrait,portrait,csshp, hp,"横屏提示"
|  cssfont  |  web自定义字体 关键字: cssfont, font,"字体引入","字体"
|  csscdbg  |  噪点背景 关键字: "csscdbg","cdbg","cssbg","bg"
|  csscoderainbg  |  代码雨背景 关键字: "csscoderainbg","coderainbg","cssbg","bg"
|  csscirclebg  |  圆点背景 关键字: "csscirclebg","circlebg",,"cssbg","bg"
|  cssrectbg  |  方格背景 关键字: "cssrectbg","rectbg","cssbg","bg"
|  ifplus  |  ccs样式下专为ifplus-loader定义的条件代码段 关键字: "ifplus","cssifplus"
<br />

### React代码段

|  缩写  |  模板  
|  ----  |  ----  
|  rinit  |  reac函数组件模板代码段 关键字："rinit", "init"
|  rinitclass  |  react类组件模板代码段 关键字："rinitclass", "initclass"
|  rdiv  |  带className的标签模板 关键字："rdiv" , "div"
|  r&&  |  &&条件渲染 关键字："r&&", "&&"
|  r?/r3m  |  react三目运算条件渲染 关键字："r?", "r3m"
|  ron  |  react常用Dom事件 关键字："ron", "on"
|  rstyle  |  react行间样式写法 关键字："rstyle", "style"
|  rroot  |  react生成React.Fragment <>根节点 关键字："rroot","root"
|  rhtml  |  react html渲染 关键字："rhtml", "html"
|  ruseState   |  useState片段  关键字："usestate", "rusestate"
|  rusestatefunction   |  usestate函数形式片段  关键字："rusestatefunction", "usestatefunction"
|  ruseeffect   |  useeffect片段  关键字："ruseeffect", "useeffect"
|  rusereducer   |  useReducer代码段  关键字："rusereducer", "usereducer"
|  ruseCallback   |  useCallback代码段 关键字： "rusecallback", "usecallback"
|  ruseRef   |  useRef代码段  关键字："ruseref", "useref"
|  ruseContext   |  useContext代码段 关键字："rusecontext", "usecontext"
|  rmap   |  react map批量渲染 关键字："rmap","map"

<br />

### HTML代码段

|  缩写  |  模板  
|  ----  |  ----  
|  htmlviewport  |  mate viewport最佳实践 关键字："htmlviewport","viewport"
|  htmlseo  |  html添加描述和关键字mate 关键字："htmlseo", "seo"
|  htmlvue  |  vue单文件组件模板 关键字："htmlvue","vue"
|  htmlvfor  |  vue框架的v-for语句段 关键字："htmlvfor","vfor"
|  htmlmetatelephone | mate 关闭自动识别数字为手机号 关键字："htmltelephone","metatelephone","关掉电话识别"
|  htmlmetaemail | mate 关闭自动识别邮箱地址 关键字："htmlmetaemail","metaemail","关掉邮件识别"
|  htmlatelphone | a标签拨打电话 关键字："htmlatelphone","atelphone","打电话"
|  htmlaemail | a标签打开邮箱 关键字："htmlaemail","aemail","发邮件"
|  htmlasms | a标签发短信 关键字："htmlasms","asms","发短信"
|  htmltable | table标签 关键字："htmltable", "table"
|  htmlul | ul标签 关键字："htmlul", "ul"
|  htmldl | dl标签 关键字："htmldl", "dl"
|  htmlscript | script标签 关键字："htmlscript", "script"
|  htmlico | 网页图标 关键字："htmlico","ico","网站图标"
|  htmllinkcss | 外链css 关键字："htmllinkcss","linkcss","外链css"
|  ifplus  |  html下专为ifplus-loader定义的条件代码段 关键字："htmlifplus","ifplus"
<br />

### JSON代码段

|  缩写  |  模板  
|  ----  |  ----  
|  ifplus  |  json下专为ifplus-loader定义的条件代码段
<br />

### Markdown代码段

|  缩写  |  模板  
|  ----  |  ----  
|  mdh1  |  一级标题 关键字："mdh1","h1"
|  mdh2  |  二级标题  关键字："mdh2","h2"
|  mdh3  |  三级标题  关键字："mdh3","h3"
|  mdol  |  无序列表  关键字："mdol","ol"
|  mdul  |  有序列表  关键字："mdul","ul"
|  mdimg  |  图片插入  关键字："mdimg","img"
|  mdlink  |  链接插入  关键字："mdlink","link"
|  mdtable  |  表格插入  关键字："mdtable","table"
|  mdb  |  粗体文字  关键字："mdb","b"
|  mdi  |  斜体文字  关键字："mdi","i"
|  mddel  |  删除文本  关键字："mddel","del"
|  mdcode  |  引入代码块  关键字："mdcode","code"
|  mdtodo  |  输入todolist  关键字："mdtodo","todo"
<br />

### 全局代码段

|  缩写  |  模板  
|  ----  |  ----  
|  gbtesttxt  |  生成中文占位文本 关键字："gbtesttxt","testtxt","中文占位文字","占位文字"
|  gbtesttxten  |  生成英文占位文本 关键字："gbtesttxten","testtxten","英文占位文字","占位文字"
|  gbtestdate  |  生成日期占位文字 关键字："gbtestdate","testdate","日期占位文字","占位文字"
|  gbtestimg  |  生成测试占位图片dummyimage.com 关键字："gbtestimg","testimg","占位图片"
|  gbtestimg0  |  生成测试占位图片fakeimg.pl 关键字："gbtestimg","testimg","占位图片"
|  gbgitignore  |  git忽略常用配置 关键字："gbgitignore","gitignore","git忽略配置"
|  gbnpmregistry  |  npm常用国内源 关键字："gbnpmregistry","npmregistry","npm源"
|  gbbaidu  |  baidu搜索 关键字："gbbaidu","baidu"
|  gbvue  |  vue官网链接 关键字："gbvue","vue"
|  gbreact  |  react官网链接 关键字："gbreact","react"
|  gbnextjs  |  nextjs官网链接 关键字："gbnextjs","nextjs"
|  gbtaro  |  taro官网链接 关键字："gbtaro","taro"
|  gbweixin  |  weixin官方文挡 关键字："gbweixin","weixin"
|  gbwebpack  |  webpack官网链接 关键字："gbwebpack","webpack"
|  gbvite  |  vite官网链接 关键字："gbvite","vite"
|  gbantdesign  |  ant design官网链接 关键字："antdesign","gbantdesign"
|  gbelementui  |  elementui官网链接 关键字："gbelementui","elementui"
|  gbgsap  |  gsap官网链接 关键字："gbgsap","gsap"
