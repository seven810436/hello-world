<!DOCTYPE html>
<html>
<head>
<meta charset="utf-8" />
<title>HTML总结</title>
</head>

<body>
    <h1 align="center">HTML总结</h1>
<ol type="A">
      <li><h2><abbr title="Hyper Text Markup Language">HTML</abbr>：超文本标记语言（Hyper Text Markup Language）。</h2></li>
  <p>标记语言由标记标签组成，标记标签的作用是描述网页。HTML文档也称为WEB页面，由标签和文本组成。</p>
  <p><abbr title="HTML tag">HTML标签</abbr>：</p>
      <ol type="I">
            <li>由尖括号包围的关键词组成</li>
            <li>成对出现，第一个是开始标签，第二个是结束标签。例如：&lt;标签&gt;内容&lt;/标签&gt;</li>
      </ol>
  <p>从某种意义上讲：HTML标签==HTML元素</p>
      <li><h2>HTML页面结构（&lt;html&gt;定义整个文档）</h2></li>
      <div style="width:500px; height:380px; background-color:#666;">
      <pre>
      &lt;!DOCTYPE html&gt;
      &lt;html&gt;
          &lt;head&gt;
              &lt;meta charset="UTF-8"&gt;
              &lt;tittle&gt;页面标题&lt;/tittle&gt;
          &lt;/head&gt;
          <div style="width:400px; height:180px; background-color:#FFF; margin:auto;">
          &lt;body&gt;
              &lt;h1&gt;一级标题&lt;/h1&gt;
              &lt;p&gt;段落一&lt;/p&gt;
              &lt;p&gt;段落二&lt;/p&gt;
          &lt;/body&gt;
          <p style=" color:#F00">白色区域是浏览器中显示区域所要显示的内容。</p>
          </div>
        &lt;/html&gt;
      </pre>
      </div>
      <p>&lt;!DOCTYPE&gt;声明有助于浏览器正确显示网页，且不区分大小写，声明文档类型，常用：&lt;!DOCTYPE html&gt;</p>
      <p>为避免页面中中文乱码，在&lt;head&gt;标签中声明：&lt;meta charset="UTF-8"&gt;</p>
      <li><h2>HTML基础</h2></li>
      <dl>
      <dt><strong>HTML标题</strong></dt>
      <dd>由&lt;h1&gt;&mdash;&lt;h6&gt;来定义，字体逐渐变小。</dd>
      <strong>例如：</strong>
      <h1 class="noshadow">一级标题</h1>
      <h2 class="noshadow">二级标题</h2>
      <h3>三级标题</h3>
      <h4>四级标题</h4>
      <h5>五级标题</h5>
      <h6>六级标题</h6>
      <dt><strong>HTML段落</strong></dt>
      <dd>由&lt;p&gt;标签来定义。</dd>
      <dt><strong>HTML链接</strong></dt>
      <dd>由&lt;a&gt;来定义，&lt;a href="http://..."&gt;</dd>
      <strong>例如：</strong><a href="https://www.hao123.com/" style="text-decoration:none;">点击进入好123导航网站</a>
      <strong>或者</strong><a href="https://www.baidu.com"><img src="../img/搜狗截图20160815164731.png" /></a>
      <dt><strong>HTML图像</strong></dt>
      <dd>由&lt;img&gt;来定义，&lt;img src="源地址" alt="当图片失效时的替换文字或其他"&gt;</dd>
      <strong>例如：</strong><img src="../img/Img449692199.jpeg" alt="图片已失效" style="width:150px; height:150px;" />
      </dl>
      <li><h2>HTML元素的语法与属性</h2></li>
      <h3>HTML元素的语法</h3>
      <ol>
      <li>以开始标签起始，以结束标签终止。</li>
      <li>元素的内容在两个标签之间。</li>
      <li>空标签在开始标签中进行关闭。</li>
      <li>元素可以拥有属性。</li>
      </ol>
      <h3>HTML属性：是HTML元素所提供的附加信息。</h3>
      <ol>
      <li>HTML元素可以设置属性。</li>
      <li>可在元素中添加附加信息。</li>
      <li>属性一般描述于开始标签。</li>
      <li>属性总以 <strong>名称=“值”</strong> 的形式出现。</li>
      </ol>
      <p>HTML注释，&lt;!--注释文字--&gt;</p>
      <p>HTML水平线，&lt;hr/&gt;</p><hr />
      <p>HTML折行，<br />&lt;br/&gt;</p>
      <p><em>&lt;em&gt;斜体字&lt;/em&gt;</em><br /><strong>&lt;strong&gt;粗体字&lt;/strong&gt;</strong><br /><small>&lt;small&gt;小号字&lt;/small&gt;</small><br /><sub>&lt;sub&gt;下标字&lt;/sub&gt;</sub><sup>&lt;sup&gt;上标字&lt;/sup&gt;</sup><br /><ins>&lt;ins&gt;插入字&lt;/ins&gt;</ins><br /><del>&lt;del&gt;删除字&lt;/del&gt;</del><br /><address>&lt;address&gt;地址&lt;/address&gt;</address><br /><blockquote>&lt;blockquote&gt;这是一段长引用。&lt;/blockquote&gt;</blockquote><br /><q>&lt;q&gt;短引用&lt;/q&gt;</q></p>
      <p>&lt;base&gt;元素描述了基本的链接地址，该标签作为HTML文档中所有链接标签的默认地址。</p>
      <base href="https://www.hao123.com/" target="_blank" />
      <a href="">链接一没有指定地址</a>
      <p>&lt;link&gt;元素链接外部资源，如样式表。<br />&lt;link rel="stylesheet" type="text/css" href="地址及文件"/&gt;</p>
      <p>&lt;style&gt;元素内部样式表。</p>
      <pre>
      &lt;head&gt;
      &lt;style type="text/css"&gt;
          body {...}
          p {...}
      &lt;/style&gt;
      &lt;/head&gt;
      </pre>
      <li><h2>HTML表格：由&lt;table&gt;来定义，由&lt;caption&gt;来定义表格标题，由&lt;th&gt;来定义表头，由&lt;tr&gt;来定义表的每一行，由&lt;td&gt;来定义表的单元格。</h2></li>
  <div style="width:300px; height:200px;">
      <pre>
      &lt;table&gt;
        &lt;caption&gt;...&lt;/caption&gt;
        &lt;tr&gt;
          &lt;th&gt;...&lt;/th&gt;
        &lt;/tr&gt;
        &lt;tr&gt;
          &lt;td&gt;...&lt;/td&gt;
        &lt;/tr&gt;
      &lt;/table&gt;
      </pre>
      </div>
  <table border="1px" bordercolor="#FF0000" cellspacing="0" cellpadding="5px">
      <caption>七八月营收状况</caption>
      <tr>
      <th>月份</th><th colspan="2">营收</th>
      </tr>
      <tr>
      <th>收支</th><td>收入</td><td>支出</td>
      </tr>
      <tr>
      <th>7月</th><td>130</td><td>50</td>
      </tr>
      <tr>
      <th>8月</th><td>160</td><td>80</td>
      </tr>
      <tr>
      <th>总和</th><td>290</td><td>130</td>
      </tr>
      </table>
      <p>单元格跨列：&lt;th/td clospan="所跨格数"&gt;</p>
      <p>单元格跨行：&lt;th/td rowspan="所跨行数"&gt;</p>
      <p>单元格边距：&lt;table border="值" cellpadding="值"&gt;</p>
      <p>单元格间距：&lt;table border="值" cellspacing="值"&gt;</p>
      <p>&lt;thead&gt;定义表格页眉。<br />&lt;tbody&gt;定义表格主体。<br />&lt;tfoot&gt;定义表格页脚。</p>
      <li><h2>HTML列表</h2></li>
      <ol>
      <li>无序列表，用style属性定义不同类型的列表，style="list-style-type:disc/circle/square"</li>
      <li>有序列表，用type属性定义不同类型的有序列表，用start属性定义从不同数字或字母开始排序。</li>
      <li>自定义列表由项目和注释组成，以&lt;dl&gt;开始，以&lt;dt&gt;定义项目，以&lt;dd&gt;定义注释。</li>
      </ol>
      <li><h2>块级元素block-level和内联元素inline（行级元素）</h2></li>
      <p>1.块级元素通常以新行开始和结束，如：&lt;h1&gt;,&lt;p&gt;,&lt;table&gt;<br />2.内联元素（行级元素）不会以新行开始，如：&lt;a&gt;,&lt;img&gt;,&lt;span&gt;<br />3.&lt;div&gt;元素：用于组合其他HTML元素的容器，常用于文档布局。</p>
      <li><h2>HTML表单：是一个包含表单元素的区域，由&lt;form&gt;定义。</h2></li>
      <p>1.表单元素：允许用户在表单中输入内容，如：文本域、下拉列表、单选框、复选框等等。<br />2.文本域，由&lt;textarea rows="行数" cols="列数"&gt;文本&lt;/textarea&gt;<br />3.文本框，由&lt;input type="text"&gt;定义。<br />4.密码字段，由&lt;input type="password"&gt;定义。<br />5.单选按钮，由&lt;input type="radio"&gt;定义。<br />6.复选框，由&lt;input type="checkbox"&gt;定义。（单选和复选中当checked="checked"时为默认选中。）<br />7.提交按钮，由&lt;input type="submit"&gt;定义。<br />8.&lt;lable&gt;标签改进鼠标用户的可用性，当鼠标点击&lt;lable&gt;中的文本时，会自动将光标焦点转移到相关的表单控件上,&lt;lable for="控件id名称"&gt;<br />9.&lt;input&gt;中的name为控件名，value为默认值（name,value主要供后端使用），当value为输入框或文本域的属性时，起提示作用。<br />10.下拉列表由&lt;select&gt;定义，当selected="selected"时为默认选中。<br />11.创建按钮，&lt;input type="button" value="按钮名称"&gt;<br />12.&lt;fieldset&gt;定义了相关的表单元素，并使用外框包含起来。&lt;legend&gt;定义了&lt;fieldset&gt;元素的标题。</p>
      <label for="username">用户名：</label><input name="username" value="请输入您的用户名" type="text" /><br />
      <label for="password">密&nbsp;&nbsp;码：</label><input name="password" value="请输入您的密码" type="password" /><br />
      <label for="sex">性别：</label><input name="sex" type="radio" value="male" checked="checked" />男<input name="sex" type="radio" value="female" />女<br />
      <label for="hobby">爱好：</label><input name="hobby" type="checkbox" checked="checked" />乒乓球</label><input name="hobby" type="checkbox"  />羽毛球</label><input name="hobby" type="checkbox"  />篮球</label><input name="hobby" type="checkbox"  />网络游戏</label><input name="hobby" type="checkbox" />旅游</label><input name="hobby" type="checkbox"  />跑步<br />
      <label for="cars">汽车品牌：</label>
      <select name="cars">
      <option value="ad" selected="selected">奥迪</option>
      <option value="dz">大众</option>
      <option value="bm">宝马</option>
      <option value="bc">奔驰</option>
      <option value="tsl">特斯拉</option>
      </select>
  <input name="submit" type="submit" value="提交" /><input name="reset"  type="reset" value="重置" />
      <fieldset>
      <legend align="center">邮件</legend>
      <label for="email">邮箱：</label><input name="email" type="email" value="810436051@qq.com" />
      </fieldset>
      <li><h2>HTML框架：通过使用框架可以在浏览器中显示不止一个页面。</h2></li>
     <p>由&lt;iframe&gt;定义，&lt;iframe src="URL"&gt;&lt;/iframe&gt;,用width和height来定义框架的宽和高，iframe属性中的iframeborder定义是否显示边框。当iframeborder="0"时移除边框。</p>
     <p>也可以将目标链接中的页面显示到框架中。<br />&lt;iframe src="URL" name="iframe_a"&gt;&lt;/iframe&gt;<br />&lt;a href="目标链接" target="iframe_a"&gt;链接&lt;/a&gt;</p>
     <iframe src="URL" name="iframe_a" style="width:800px; height:450px;"></iframe>
     <a href="https://www.hao123.com/" target="iframe_a">点击此链接显示在框架中</a>
     <li><h2>HTML脚本</h2></li>
     <p>&lt;script&gt;标签：用于定义客户端脚本文件，可以包含脚本语句，也可通过SRC外链脚本文件。Javascript常用于图片操作，表单验证及内容动态更新。<br />&lt;noscript&gt;标签：提供无法使用脚本文件时的替代内容。</p>
     <li><h2>字符实体</h2></li>
  <table border="1px" bordercolor="#0000FF" cellpadding="15px" cellspacing="0" style="text-align:center">
     <tr>
     <th>字符</th><th>代码</th><th>字符</th><th>代码</th>
     </tr>
     <tr>
     <td>不间断空格</td><td><abbr title="no-breaking space">&amp;nbsp； </abbr></td><td>&copy;</td><td>&amp;copy； </td>
     </tr>
     <tr>
     <td>&lt;</td><td> &amp;lt； </td><td>&reg;</td><td>&amp;reg； </td>
     </tr>
     <tr>
     <td>&gt;</td><td>&amp;gt； </td><td>&trade;</td><td>&amp;trade； </td>
     </tr>
     <tr>
     <td>&amp;</td><td>&amp;amp； </td><td>&times;</td><td>&amp;times； </td>
     </tr>
     <tr>
     <td>&yen;</td><td>&amp;yen； </td><td>&divide;</td><td>&amp;divide； </td>
     </tr>
     </table>
     <li><h2><abbr title="（Uniform Resource Locators）">URL</abbr>统一资源定位器（Uniform Resource Locators）</h2></li>
  </ol>
</body>
</html>
