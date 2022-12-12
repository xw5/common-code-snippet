# 开发常用代码段插件
>根据缩写快速提供代码模板，提高开发速度，代码段持续更新中......
<br />

## 使用建议
>考虑到用户的记忆成本，用户无需记忆所有代码段的缩写，输入特殊开头字符则会带出当前类别下的代码段，优化使用体验，定义如下使用规则：
>- 在js/jsx下输入js则会带出所有属于js的代码段,输入taro就带出taro特有的代码段（注：有些taro代码段只有jsx下才会有）
>- css下输入css则会带出所有属于css的代码段
>- html下输入html会带出所有属于html的代码段
>- mardown下输入md会带出所有属于markdown的代码段
>- 全局输入gb(global的缩写)会带出全局的代码段
>- 支持不带特殊符号的输入形式：如cssellipsis和ellipsis都能带出css下单行省略号的代码段
>- 代码段匹配字段都会尽量使用语义化的字段,如mdol:在mardown下输入无序列表;cssarrowtop:css实现的向上箭头，这样可以让用户记忆不再有太大负担

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
|  jsvar  |  js 定义变量代码段
|  jsfor  |  js for基本用法
|  jsforof  |  for-of循环
|  jsforin  |  for-in循环
|  jsif  |  if语句
|  jsifelse  |  if下的else语句
|  jselseif  |  if下的elseif语句
|  jsswitch  |  js下switch语句
|  jstry  |  js下try catch语句
|  jsfunction  |  js function定义结构
|  jslog  |  js下console.log语句
|  jsinfo  |  js下console.info语句
|  jserror  |  js下console.error语句
|  jsclass  |  js 类定义结构
|  jspromise  |  js Promise定义结构
|  regexcommon  |  常用正则表达式集合(用户名、密码、手机号、邮箱、身份证...)
|  jsthrottle  |  js下节流代码段
|  jsdebounce  |  js下防抖代码段
|  jsstore  |  vue状态管理主文件模板代码段
|  jsstoremodule  |  vue状态管理module模板代码段
|  jsdialogdrag  |  el弹窗拖拽指令
|  jsrem   |  移动端rem计算代码段 
|  jsuseState   |  useState片段 
|  jsusestatefunction   |  usestate函数形式片段 
|  jsuseeffect   |  useeffect片段 
|  jsusereducer   |  useReducer代码段 
|  jsuseCallback   |  useCallback代码段 
|  jsuseRef   |  useRef代码段 
|  jsuseContext   |  useContext代码段 
|  jsimport   |  import{}语句代码段 
|  jsimportdefault   |  importdefalt语句代码段 
|  jscsfn  |  js const定义箭头函数代码段 
|  js?  |  js 三目运算代码段
|  jsArraymethod  |  Array常用方法列表
|  jsStringMethod  |  String常用方法列表
|  jsMathMethod  |  Math对象常用方法
|  jsDateMethod  |  Date常用方法
|  jsLocation  |  Location对象属性和方法
|  jsHistory  |  History对象方法
|  jsDom  |  Dom元素对象
|  tarohide  |  taro toaset loading隐藏
|  taronavigate  |  taro的路由跳转api代码段
|  tarocliboard  |  剪贴板操作api
|  tarosetstorage  |  设置key:data本地缓存
|  tarogetstorage  |  获取指定key的本地缓存
|  tarosetstoragesync  |  同步方式设置key:data本地缓存
|  tarogetstoragesync  |  同步方式获取指定key的本地缓存
|  taroremovestoragesync  |  同步方式删除指定key的本地缓存
|  taroremovestorage  |  异常方式删除指定key的本地缓存
|  taroshowtoast  |  taro showToast显示消息提示框
|  taroshowmodel  |  taro showModel显示模态对话框
|  taroshowloading  |  taro showLoading显示消息提示框
|  ifplus  |  js代码下专为ifplus-loader定义的条件代码段 
<br />

### jsx代码模板
> Javascript代码模板一样可以使用

|  缩写  |  模板  
|  ----  |  ----  
|  taropage  |  taro page组件模板
|  tarocomponent  |  taro component模板
|  taropageconfig  |  taro page配置模板
|  tarousehook  |  taro 特有hooks

<br />

### CSS代码段

|  缩写  |  模板  
|  ----  |  ----  
|  cssellipsis  |  单行文本超出省略号
|  cssreset  |  css样式重置
|  cssellipsismulti  |  多行文本超出省略号
|  csswrap  |  css强制换行
|  cssarrowtop  |  css实现朝上箭头
|  cssarrowbottom  |  css实现朝下箭头
|  cssarrowleft  |  css实现朝左箭头
|  cssarrowright  |  css实现朝右箭头
|  cssgray  |  置灰滤镜
|  cssblur  |  模糊滤镜
|  csscenterflex  |  flex方式子元素水平垂直居中
|  csscentermargin  |  absolute+margin元素水平垂直居中
|  csscentertransform  |  absolute+transform元素水平垂直居中
|  cssplaceholder  |  设置input的placeholder的颜色
|  cssmedia  |  media媒体查询参考段
|  cssgradient  |  css渐变参考写法
|  cssNoSelect  |  css禁止文本选中
|  cssslectioncolor  |  设置选区背景颜色
|  cssflex  |  display:flex
|  cssflexcolumn  |  flex column
|  cssflexcenter  |  flex水平垂直居中
|  csslink  |  a链接伪类设置顺序
|  css::border  |  css伪类实现边框
|  cssboxshadow  |  css boxshadow盒子阴影
|  csstransition  |  css transition过渡
|  csskeyframes  |  css keyframes动画定义
|  ifplus  |  ccs样式下专为ifplus-loader定义的条件代码段
<br />

### HTML代码段

|  缩写  |  模板  
|  ----  |  ----  
|  htmlviewport  |  mate viewport最佳实践
|  htmlseo  |  html添加描述和关键字mate
|  htmlvue  |  vue单文件组件模板
|  htmlvfor  |  vue框架的v-for语句段
|  ifplus  |  html下专为ifplus-loader定义的条件代码段
|  htmlmetatelephone | mate 关闭自动识别数字为手机号
|  htmlmetaemail | mate 关闭自动识别邮箱地址
|  htmlatelphone | a标签拨打电话
|  htmlaemail | a标签打开邮箱
|  htmlasms | a标签发短信
<br />

### JSON代码段

|  缩写  |  模板  
|  ----  |  ----  
|  ifplus  |  json下专为ifplus-loader定义的条件代码段
<br />

### Maekdown代码段

|  缩写  |  模板  
|  ----  |  ----  
|  mdh1  |  一级标题
|  mdh2  |  二级标题
|  mdh3  |  三级标题
|  mdol  |  无序列表
|  mdul  |  有序列表
|  mdimg  |  图片插入
|  mdlink  |  链接插入
|  mdtable  |  表格插入
|  mdb  |  粗体文字
|  mdi  |  斜体文字
|  mddel  |  删除文本
|  mdcode  |  引入代码块
|  mdtodo  |  输入todolist
<br />

### 全局代码段

|  缩写  |  模板  
|  ----  |  ----  
|  gbtesttxt  |  生成中文占位文本
|  gbtesttxten  |  生成英文占位文本
|  gbtestdate  |  生成日期占位文字
|  gbtestimg  |  生成测试占位图片
|  gbbaidu  |  baidu搜索
|  gbvue  |  vue官网链接
|  gbreact  |  react官网链接
|  gbreact  |  react官网链接
|  gbnextjs  |  nextjs官网链接
|  gbtaro  |  taro官网链接
|  gbweixin  |  weixin官方文挡
|  gbwebpack  |  webpack官网链接
|  gbvite  |  vite官网链接
|  gbantdesign  |  ant design官网链接
|  gbelementui  |  elementui官网链接
|  gbgsap  |  gsap官网链接
