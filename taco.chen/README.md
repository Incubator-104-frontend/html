# HTML
![HTML DOM model](https://www.w3schools.com/js/pic_htmltree.gif)
- id can actually be used more than once but should only be used once
    - like we have an unique identification
- div / p / header / footer / section / nav (default block element)
    - block element extend the width to 100%(inherit the width from parent element)
- a / span (default inline element)
## nav
- define a set of navigation links
## HTMLFormElement
- provide method to create and modify form element
- get form element & form input
    - document.forms["id" / "name"]
    - document.forms[""].name.value
## html tag
### text content
* q 
    * inline element
    * short quotation
    * built-in pseudo element content for open closed quote
    * q in p
* blockquote
    * block element
    * long quotation
    * p in blockquote
* dl dt dd
    * block element
    * dl description list
    * dt description term
    * dd description
    * usually used for description of terminology
        - multiple / single term with multiple / single description
* hr
    * block element
    * break between paragraph-level element
    * built-in attribute
        - width size(height) color etc...
* ol ul li
    * ordered list / unordered list
* div
    * block element container
* p
    * p inside p is invalid
##  
* figure
    * include not just image or video but also description
* figcaption
    * represent title of figure
## 
### content sectioning
* section
    * block element
    * divider to separate a document which are related to each other
* article
    * block element
    * a text block that is unrelated to the other blocks on the page
    * section in article
        * new article with many related sections
    * article in section
        * new section with many unrelated article
* address
    * block element
    * font-style italic
    * default width 100%
    * supply contact information of its nearest article
* footer
    * block element
    * contain information about the author of the section, copyright data or link to related document
    * can include address
    * usually one footer for whole document and one footer for every section
### inline text semantic
* inline element
* span
    * no inherent meaning
    * like div for inline element container
* abbr
    * used for abbreviation
    * title attribute for definition of abbreviation
* i b em strong
    * i b means stylingthe element not for emphasizing
        * i for italic
        * b for bold
    * em strong means emphasizing
        * em for italic
        * strong for bold
    * same effect
* bdo
    * bidirectional override
    * dir attribute of ltr(left to right) rtl(right to left)
* bdi
    * bidirectional isolation
* ruby rp rt
    * show pronunciation of East Asian character
```
<ruby>
  漢 <rp>(</rp><rt>Kan</rt><rp>)</rp>
  字 <rp>(</rp><rt>ji</rt><rp>)</rp>
</ruby>
```
* br wbr
    * br force a line break
    * wbr => word break opportunity
    * if a line is too long, break the line or word at appropriate position
    * avoid horizontal scroll
##
* kbd
    * represent user keyboard input
    * default font-family monospace 
* code
    * represent a partion of programming code
    * default font-family monospace
* samp
    * represent sample output from programming code
    * default font-family monospace
* var
    * represent variable in mathematical expression or programming code
    * default font-style italic
        * font-style only oblique / italic or normal
##
* s
    * represent the text no longer accurate
    * render text with strikethrough(delete line)
    * default text-decoration line-through
    * unapporpriate to indicate document edition
        * using del & ins tag
* u
    * render text with underline
    * default text-decoration underline
    * label the name in Chinese text or lebel the misspelled text
    * no recommendation
* time
    * represent time
    * datetime attribute
* data
    * define value for given content
    * datetime content using time tag
* small
    * render text with font-size one size smaller
        * large to medium or medium to small etc...
    * used for copyright
##
* sup
    * change position of text to be higher and smaller
    * default vertical-align super & font-size smaller
    * used for mathematical
* sub
    * change position of text to be lower and smaller
    * default vertical-align sub & font-size smaller
    * used for mathematical or chemical formula
##
* mark
    * represent highlight text
    * show relevance and not for importance
    * default background-color yellow & color black
    * e.g show search result to highlight every instance of the searched-for word
* dfn
    * represent the definition of term
    * default font-style italic
    * sometimes abbr tag inside or used with inside p or dt dd pair
* cite
    * represent reference title of work or URL reference
    * default font-style italic
* a
    * create hyperlink
    * target attribute for loading type
        * _self default same page
        * _blank new tab
        * _parent parent page
### table content
* table
    * attribute
        * align left(default) center right
            * replaced by margin-right auto / margin 0 auto / margin-left auto
        * bgcolor
            * replaced by background-color
        * border 
            * replaced by border for table,td,th
        * cellpadding
            * define the space between the content of cell and border
            * replaced by padding for td,th
        * cellspacing
            * define the space between two cells
            * replaced by border-spacing
            * if set border-collapse to collapse, then border-spacing no effect
                * borders are collapsed into one border
* caption
    * represent title of table
    * width auto-fitting width of table
* colgroup col
    * colgroup represent all columns
    * col represent single column
    * if col inside colgroup, then span attribute only be used for col
    * allow CSS for specific column
* thead
    * represent rows defining the header of table element
* tbody
    * represent rows defining the body of table element
* tfoot
    * represent rows defining the footer of table element