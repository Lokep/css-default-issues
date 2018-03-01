# -
部分默认样式的修改，定期更新
----

# 滚动条样式修改，没有找到修改火狐浏览器滚动条的代码

## 以下为
* 谷歌、
* safari、
* qq浏览器、
* 360浏览器滚动条样式和ie滚动条样式及ie原始默认样式

`谷歌`、`safari`、`qq浏览器`、`360浏览器极速模式`滚动条样式
/*定义滚动条高宽及背景 高宽分别对应横竖滚动条的尺寸*/
```css
::-webkit-scrollbar  
{  
    width: 10px;  
    height: 10px;  
    background-color: #F5F5F5;  
}  
/*定义滚动条轨道 内阴影+圆角*/  
::-webkit-scrollbar-track  
{  
    -webkit-box-shadow: inset 0 0 6px rgba(0,0,0,0.3);  
    border-radius: 10px;  
    background-color: #F5F5F5;  
}    
/*定义滑块 内阴影+圆角*/  
::-webkit-scrollbar-thumb  
{  
    border-radius: 10px;  
    -webkit-box-shadow: inset 0 0 6px rgba(0,0,0,.3);  
    background-color: #bdbdbd;  
}  
/*滑块效果*/
::-webkit-scrollbar-thumb:hover
{
border-radius: 5px;
-webkit-box-shadow: inset 0 0 5px rgba(0,0,0,0.2);
background: rgba(0,0,0,0.4);
}
```

## IE滚动条颜色
```css
/*IE滚动条包括了 IE 360浏览器中的兼容模式*/
html {
    scrollbar-face-color:#bfbfbf;/*滚动条颜色*/
    scrollbar-highlight-color:#000;
    scrollbar-3dlight-color:#000;
    scrollbar-darkshadow-color:#000;
    scrollbar-Shadow-color:#adadad;/*滑块边色*/
    scrollbar-arrow-color:rgba(0,0,0,0.4);/*箭头颜色*/
    scrollbar-track-color:#eeeeee;/*背景颜色*/
}
```
#input-placeholder-issues
##有关placeholder设置属性

```css
input::-webkit-input-placeholder{
    color:red;
}
input::-moz-placeholder{   /* Mozilla Firefox 19+ */
    color:red;
}
input:-moz-placeholder{    /* Mozilla Firefox 4 to 18 */
    color:red;
}
input:-ms-input-placeholder{  /* Internet Explorer 10-11 */ 
    color:red;
}

```

##其他
```css
input,textarea{
   -webkit-appearance:none;
   outline:none;/*聚焦时候 的 边框*/
   border:1px solid black;
}
textarea{
   resize:none;/*无法缩放*/
}
```
