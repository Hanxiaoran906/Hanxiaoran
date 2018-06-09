# 进入前端大门时碰到的小小小坎儿

   > 笔者记  从几个月前决定开始转行前端到现在，各处搜罗视频、书籍资料慢慢学习。因资源驳杂，学习不成体系，部分知识学过几遍，也漏掉不少知识。学习期间自然也遇到一些小问题或难以理解的知识点，总是随手记在了笔记本上，或者视频学习网站的笔记上，每每想去查阅的时候总是会浪费不少时间。所以我还是整理一番，记录在这个从来没用过的博客（?）上吧（笑）。

## HTML（5）部分

### HTML4元素

   HTML4共包含91个元素，这些元素都是针对特定内容、结构或特性定义的。具体分为：
    
  结构元素：div,span,ol,ul,li,dl,dt,dd,del,ins,h1~h6,p,hr......  
  内容元素：a,abbr,acronym,address,dfn,kbd,samp,var,tt,code,pre,blockquote,cite,q,strong,em......  
  修饰元素：b,i,big,small,sup,sub,bdo,br......

### HTML4属性

  核心属性：class,id,style  
  语言属性：lang(定义元素的语言代码或编码）,dir（定义文本方向，ltr和rtl）  
  键盘属性：accesskey(定义访问某元素的键盘快捷键），tabindex（定义元素的Tab键索引编号）  
  内容属性：alt,title,longdesc,cite,datetime......  
  延展属性：rel:定义当前页面与其他页面的关系；  
           rev:定义其他页面与当前页面之间的链接关系
         
### HTML5新增元素

  结构元素：  
  header,footer,section,article,aside,nav,main,figure...  
  功能元素：  
        hgroup  : 对标题进行组合；  `<hgroup>...</hgroup>`  
        video   : 定义视频；  `<video src="movie.ogg" controls="controls">video元素</video>`  
        audio   : 定义音频；  `<audio src="audio.wav">audio元素</audio>`  
        embed   : 用来插入各种多媒体（Midi,Wav,AIFF,AU,MP3）；  `<embed src="horse.wav" />`  
        mark    : 高亮显示关键字；  `<mark></mark>`  
        dialog  : 定义对话框或窗口；  `<dialog open>这是打开的对话窗口</dialog>`  
        bdi     : 定义文本的文本方向，使其脱离其周围文本的方向设置（不受父元素文本方向的影响）  
        figcaption: 定义figure元素的标题；  
        time    : 表示日期或时间；  
        canvas  : 表示图形，如图表和其它图像。这个元素本身没有行为，仅提供一块画布，但它把一个绘图API展现给客户端JavaScript，  
                以使脚本能够把想绘制的东西绘制到这块画布上。  `<canvas id="myCanvas" width="200" height="200"></canvas>`  
        output  : 表示不同类型的输出；  `<output></output>`  
        source,menu,rt,rp,wbr,command,details,summary,datalist,datagrid,keygen,progress,meter,track......  
  表单元素：  
         通过type属性，HTML5为input元素新增了很多类型，如下:  
        tel, search, url, email, datetime, date, month, week, time, datetime-local, number, range ,color...  
        格式：`<input type="ele" />`  

### HTML5属性
  表单属性：  
        autofocus：自动获得焦点；  
        placeholder：对用户的输入进行提示；  
        form：声明它属于哪个表单；  
        required：（text与textarea）检查该元素内一定要有内容才允许提交；  
        为input元素增加autocomplete、min、max、multiple、pattern和step属性。同时还有一个新的list元素与datalist元素配合使用。datalist元素与autocomplete属性配合使用。multiple属性允许在上传文件时一次上传多个文件。  
        为input元素、button元素、form元素增加了novalidate属性，该属性可以取消提交时进行的有关检查，表单可以被无条件地提交。  
  链接属性、其他属性...  
  
### HTML5全局属性

contentEditable : 主要功能是允许用户可以在线编辑元素中的内容；是一个布尔值，可以定义为false或true。  
contextmenu : 用于定义`<div>`元素的上下文菜单，在用户右键单击元素时出现。//只有Firefox支持  
data-* : 可以自定义用户数据。  
draggable : 定义元素是否可以被拖动，true、false、auto。  
dropzone : 定义在元素上拖动数据时，是否复制、移动或链接被拖动数据。//值为：copy,move,link（不被支持）  
hidden : 用于设置元素的可见状态，取值为布尔值。eg：`<p hidden>这个段落应该被隐藏</p>`//除了IE，均支持  
spellcheck : 定义是否对元素进行拼写和语法检查，取值为布尔值。  
translate : 定义是否应该翻译元素内容，取值为yes，no。//目前不受支持  


## CSS（3）部分

#### CSS选择器的权重问题
通配符选择器 * ： 0；  
元素选择器 Tag ： 1；  
类（class）选择器 ：10；  
ID选择器 ： 100；  
行内样式 ： 1000；  
！important ： 最高。  

#### 元素竖向的百分比设定
*元素height属性取值百分比，是相对于容器高度取值。  
*元素的竖直方向的内外边距取值百分比，参考的是容器的宽度，而不是高度。  
<pre>
eg：.container{
         width:200px; height:100px;
    }
    .box{
         margin-top:20%; height:50%;
    }
</pre>
则box的高度为100px；而上外边距为40px。



## JavaScript部分
