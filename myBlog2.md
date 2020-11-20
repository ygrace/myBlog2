# html重难点标签
## a标签的用法
1. 外部页面跳转
   * 属性一 href取值接网址
     https://google.com

     http://google.com

     //google.com  自动选择
   * 如果必须写一个a标签，但是什么都不让它做，就写一个：
     ~~~html
     <a href="javascript:;"></a>
     ~~~
   * 属性二 target取值
     _blank 在新窗口打开页面
     _self 默认，在当前页面打开
     _top  在最底层页面打开
     _parent 在当前页面的上一层打开
2. 跳转内部锚点
   ~~~html
   <a href="#xxx">查看</a>
   ~~~
   xxx是id，跳转到id在的位置
3. 发邮件给xxx
   ~~~html
   <a href="mailto:xxx邮件地址>发邮件给xxx</a>
4. 打电话给xxx
   ~~~html
   <a href=“tel:xxx电话号码”>打电话给xxx</a> 
   ~~~
## img标签的用法
1. 作用 发出get请求，展示一张图片
2. 属性
   * src,source的缩写，图片的路径
   * alt,如果图片加载不到，就显示alt的内容
   * height,width 只写其中一个参数，另一个就会自适应，如只写宽度。前端工程师记住永远不要让图片变细。
3. 事件
   onload/onerror 在js里面监听图片是否加载成功
   ~~~html
   <img id="xxx" width="" src="">
   xxx onload = function() {
       console.log('图片加载成功')
   };
   xxx onerror = function() {
       console.log('图片加载失败')
       xxx.src = "路径"
   }; 
   ~~~
3. 响应式 max-width: 100%   
## table标签的用法
   * table标签里面只能有三个标签，thead标签，tbody标签，tfoot标签，可以互换顺序写，但是显示的时候按照头身体脚来显示
   * tr 表行
   * th 表头
   * td 表里的数据，在tbody里
   * table-layout: auto; 根据内容调整
   * table-layout: fixed; 平均显示
   * border-collapse: collapse  合并
   * border-spacing: 0 

## 其他的标签还有很多
form标签

input标签

textarea标签

select标签


  
