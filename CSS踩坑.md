文字区不要定高度,请使用line-height 和padding 去填充间隙,让文字自由流动自动撑开盒子的高度

- 防止文字过长造成文字溢出, (防止多语言时文字bug)

ios不识别/deep/ 嵌套

```css
.wrap{
    /deep/ .class2{

       font-size:20px; //对所有子组件生效.

        /deep/ .class3{   }  
        //没有必要写多层deep 父类有deep后子类自动也会深度选择 并且这么写在firfox里会失效
    }
}
```