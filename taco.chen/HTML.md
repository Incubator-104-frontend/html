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
- q 
    - inline element
    - short quotation
    - built-in pseudo element content for open closed quote
    - q in p
- blockquote
    - block element
    - long quotation
    - p in blockquote
- dl dt dd
    - block element
    - dl description list
    - dt description term
    - dd description
    - usually used for description of terminology
        - multiple / single term with multiple / single description
- hr
    - block element
    - break between paragraph-level element
    - built-in attribute
        - width size(height) color etc...
- ol ul li
    - ordered list / unordered list
- div
    - block element container
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
* kbd
    * default font-family monospace
    * represent user keyboard input
* ruby rp rt
    * show pronunciation of East Asian character
```
<ruby>
  漢 <rp>(</rp><rt>Kan</rt><rp>)</rp>
  字 <rp>(</rp><rt>ji</rt><rp>)</rp>
</ruby>
```
* span
    * like div for inline element container