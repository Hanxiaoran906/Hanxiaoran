<h1>进入前端大门时碰到的小小小坎儿</h1>

    笔者记  从几个月前决定开始转行前端到现在，各处搜罗视频、书籍资料慢慢学习。因资源驳杂，学习不成体系，部分知识学过几遍，也漏掉不少知识。学习期间自然也遇到一些小问题或难以理解的知识点，总是随手记在了笔记本上，或者视频学习网站的笔记上，每每想去查阅的时候总是会浪费不少时间。所以我还是整理一番，记录在这个从来没用过的博客（?）上吧（笑）。

<h2>HTML（5）部分</h2>

<h3>HTML4元素</h3>
    HTML4共包含91个元素，这些元素都是针对特定内容、结构或特性定义的。具体分为：
    
  结构元素：div,span,ol,ul,li,dl,dt,dd,del,ins,h1~h6,p,hr......<br />
  内容元素：a,abbr,acronym,address,dfn,kbd,samp,var,tt,code,pre,blockquote,cite,q,strong,em......<br />
  修饰元素：b,i,big,small,sup,sub,bdo,br......<br />

<h3>HTML4属性</h4>

  核心属性：class,id,style<br />
  语言属性：lang(定义元素的语言代码或编码）,dir（定义文本方向，ltr和rtl）<br />
  键盘属性：accesskey(定义访问某元素的键盘快捷键），tabindex（定义元素的Tab键索引编号）<br />
  内容属性：alt,title,longdesc,cite,datetime......<br />
  延展属性：rel:定义当前页面与其他页面的关系；<br />
           rev:定义其他页面与当前页面之间的链接关系<br />

<h3>HTML5新增元素</h3>

  结构元素：header,footer,section,article,aside,nav,main,figure...<br />
  功能元素：<br />
        hgroup  : 对标题进行组合；  <hgroup>...</hgroup><br />
        video   : 定义视频；  <video src="movie.ogg" controls="controls">video元素</video><br />
        audio   : 定义音频；  <audio src="audio.wav">audio元素</audio><br />
        embed   : 用来插入各种多媒体（Midi,Wav,AIFF,AU,MP3）；  <embed src="horse.wav" /><br />
        mark    : 高亮显示关键字；  <mark></mark><br />
        dialog  : 定义对话框或窗口；  <dialog open>这是打开的对话窗口</dialog><br />
        bdi     : 定义文本的文本方向，使其脱离其周围文本的方向设置（不受父元素文本方向的影响）<br />
        figcaption: 定义figure元素的标题；<br />
        time    : 表示日期或时间；<br />
        canvas  : 表示图形，如图表和其它图像。这个元素本身没有行为，仅提供一块画布，但它把一个绘图API展现给客户端JavaScript，以使脚本能够把想绘制的东西绘制到这块画布上。  <canvas id="myCanvas" width="200" height="200"></canvas><br />
        output  : 表示不同类型的输出；  <output></output><br />
        source,menu,rt,rp,wbr,command,details,summary,datalist,datagrid,keygen,progress,meter,track......<br />
  表单元素：通过type属性，HTML5为input元素新增了很多类型，如下：<br />
        tel, search, url, email, datetime, date, month, week, time, datetime-local, number, range ,color...<br />
        格式：<input type="ele" /><br />

<h2>CSS（3）部分</h2>


<h2>JavaScript部分</h2>
