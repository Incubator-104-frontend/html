# CSS1
![CSS specificity](http://www.oxxostudio.tw/img/articles/201405/20140530_1_02.jpg)
## basic
* CSS built running code from top to buttom, then taking last property
* inline
    * html tag attribute
* internal
    * html head style
    * loaded earlier than inline
* external
    * html link style file
    * loaded earlier than inline
* comment /* @ start & */ @ end
* margin
    * padding outside of the element
* content
    * attr(style) attr(href) attr(class) etc
### block & inline
* block element begin from new line, spread to full container
* inline element not change original layout of paragraph
### font-size
* em relative parent element
* rem relative root element(html)
* inheritance yes
### color 
* named color
* hex color #xxxxxx 
    * #xxx browser assume repetition
    * #000000 black
    * #ffffff white
    * form 000 to fff get more transparent
* rgb colors
    * rgb / rbga in CSS3
    * rgb(0,0,0) black
    * rgb(255,255,255) white
### hover & active
* :hover selector
    * mouse over to change property
* :active selector
    * click to change property
### white-space
* default normal 
    * Sequence of whitespace collapse into one whitespace
    * text wrap when necessary
* nowrap
    * Sequence of whitespace collapse into one whitespace
    * text nevar wrap except for br tag
* pre
    * whitespace is preserved
    * text wrap only when line break or br tag
* pre-line
    * Sequence of whitespace collapse into one whitespace
    * text wrap when necessary
* pre-wrap
    * whitespace is preserved
    * text wrap when necessary
* invisible
    * display none along with JS modifying element property dynamically
        * not reserve original space
    * visibility hidden 
        * reserve original space
## position
* relative
    * position relative to its original position not affecting other element position
    * original position space remained
* fixed
    * position relative browser window position & fixed not affecting other element position
    * mobile device support low
    * original position not remained
* absolute
    * position relative to its first positioned (not static) parent element
## advanced
### float
* set overflow to auto clearing float
* clear
    * only applied to block-level element
### center vertically
* set line height equal to container height
    * only for inline(single line) / inline-block(div) with vertical-aligh middle
* add pseudo element
* calc 動態計算
    * margin using % get % of horizontal width
* flex
    * justify-content(vertical) & align-items(horizontal) set center
### flex
* one-dimensional layout
* support 
    * -webkit-box / -moz-box / -ms-flexbox / -webkit-flex
#### property for parent
* flex-flow
    * shorthand of flex-direction & flex-wrap
    * default is row nowrap
#### property for children
### grid
* two-dimensional layout
* using align-self locate single cell
### render engine 渲染引擎 (leyout engine)
* CSS-prefix
    * chrome safari
        * webkit
    * firefox
        * moz
    * IE edge
        * ms
### RWD 
## CSS design
* avoid using ID selector
    * ID's specificity too high
        * 255 times than class's specificity
        * hard to override property
    * class reusable
* avoid using magic number
    * means exactly effective number
    * replaced by % of container etc
* avoid using !important, if necessary, refactor way of selector
### selector
* 
## CSS framework
* OOCSS
    * object-oriented CSS
    * divide every feature into class
    * avoid child selector, randomly assign style to any html tag