# -
    部分默认样式的修改，定期更新

滚动条样式修改，没有找到修改火狐浏览器滚动条的代码

把以下样式加入css，图片为谷歌、safari、qq浏览器、360浏览器滚动条样式和ie滚动条样式及ie原始默认样式

'谷歌'、`safari`、`qq浏览器`、`360浏览器极速模式`滚动条样式
/*定义滚动条高宽及背景 高宽分别对应横竖滚动条的尺寸*/
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


/*IE滚动条颜色*/
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
