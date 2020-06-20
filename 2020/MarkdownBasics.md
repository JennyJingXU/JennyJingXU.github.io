# Markdown Instruction

## What is  Markdown?
    - a lightweight markup language 
    - plain-text-formatting syntax
    - a software tool, written in Perl, that converts the plain text formatting to HTML
    - to write readme file, create rich text
    - Files extension: `.md` or `.markdown` 
## Difference: Markdown vs HTML
    Markdown is not a replacement for HTML, or even close to it.
    - Markdown is a very small subset of HTML tags, addressing **writing** format  
    - HTML is a **publishing** format
    - For any markup that is not covered by Markdown’s syntax, you simply use HTML itself.   
Example:

    This is a *regular* paragraph.
    
    <table>
        <tr>
            <td>Foo</td>
        </tr>
    </table>
    
    This is another regular paragraph.
Note:
  - Block-level

        Markdown formatting syntax is not processed within block-level HTML tags 
         — e.g. <div>, <table>, <pre>, <p>, etc., 
        you can’t use Markdown-style *emphasis* inside an HTML block.
   
  - Span-leverl 

        Span-level HTML tags — e.g. <span>, <cite>, or <del> — 
        can be used anywhere in a Markdown paragraph, list item, or header. 
        If you want, you can even use HTML tags instead of Markdown formatting; 
        e.g. if you’d prefer to use HTML <a> or <img> tags instead of Markdown’s link or image syntax, 
        go right ahead.


## Why Markdown?
    - easy-to-read 
    - easy-to-write
## Syntax
### Header

    # This is an <h1> tag  
    ## This is an <h2> tag  
    ###### This is an <h6> tag

### Emphasis `*`; `_`; `~`;
Example:
    *This text will be italic*  
    _This will also be italic_

    *This text will be italic*  
    _This will also be italic_
Example:
    **This text will be bold**  
    __This will also be bold__

    **This text will be bold**  
    __This will also be bold__
Example:
    _You **can** combine them_

    _You **can** combine them_

Example:
    ***This text will be italic & bold***

    ***This text will be italic & bold***
Example:
    ~~This text will have strikethrough~~   

     ~~This text will have strikethrough~~ 


​     
### List
#### Unordered List `*` `-` `+`
* item 1
+ item 2
    * item 2a
    * item 2b
- item 3  

 Method 1: Markdown Number  
    
        * item 1
        + item 2
            * item 2a
            * item 2b
        - item 3

Method 2: HTML  
#### Ordered List `1` `2` `3`

1. item 1
    1. item 1.1
    2. item 1.2
2. item 2
3. item 3
    1. item 3a
    2. item 3b

Method 1: Markdown Number    

    1. item 1
        1. item 1.1
        2. item 1.2
    2. item 2
    3. item 3
        1. item 3a
        2. item 3b

<ol>
  <li>one</li>
  <li>two
  <ol>
      <li>inner 1</li> 
      <li>inner 2</li>
  </ol></li>  
  <li>three</li>
</ol>        
Method 2: HTML

    <ol>
      <li>one</li>
      <li>two
      <ol>
          <li>inner 1</li> 
          <li>inner 2</li>
      </ol></li>  
      <li>three</li>
    </ol>   

### Blockquotes `>`
- Blockquotes can be nested  
- Blockquotes can contain other Markdown elements, 
including headers, lists, and code blocks:

Example:  

As Kanye West said:
> We're living the future so
> the present is our past.
> >from Kanye West  `>>`
> >>This is nested blockquote `>>>`
> >>###### here is a header.
> >>1. here is the 1st list item
> >>2. here is the 2nd list item  

    As Kanye West said:
    > We're living the future so
    > the present is our past.
    >>from Kanye West  `>>`
    >>>This is nested blockquote `>>>`
    >>> ###### here is a header.
    >>>1. here is the 1st list item
    >>>2. here is the 2nd list item  
### Inline Code `` ` ``
Example: I think you should use an `<addr>` element here.

    I think you should use an `<addr>` element here.
A single backtick in a code span: `` ` ``  

    A single backtick in a code span: `` ` ``
A backtick-delimited string in a code span: `` `foo` ``  

    A backtick-delimited string in a code span: `` `foo` ``
### Code Block 
Method 1: 4 spaces  
Method 2: 1 tab  
### Horizontal Rule
*****
3 or more hyphens, asterisks, or underscores on a line   
Space is optional

    * * *
    ***
    - - -
    ---------------------------------------
### Line break
 - Method 1:  2 or more spaces, and then type return <br/>
 - Method 2:  insert a `<br/>` tag at the end
 - Method 3:  blockquoting `>`
 - Method 4: list items `*`; `-`; `+`;

## Backslash Escape 
Example: \*literal asterisks\*  

    \*literal asterisks\*

Markdown provides backslash escapes for the following characters:
    
    \   backslash
    `   backtick
    *   asterisk
    _   underscore
    {}  curly braces
    []  square brackets
    ()  parentheses
    #   hash mark
    +   plus sign
    -   minus sign (hyphen)
    .   dot
    !   exclamation mark
### Image
Example: ![Github Logo](https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png)  

    ![Github Logo](/Users/jing/Desktop/GitHub/GitHub-Mark/PNG/GitHub-Mark-64px.png)
- Format:    `![Alt Text](url)`

### Link 
 Example 1: [Github](http://github.com)    

        [Github](http://github.com)
 Example 2: <http://github.com>    

        <http://github.com>

 Format:   
   * Method 1: `![Alt Text](url)`  
   * Method 2: `<url>`  
## Advanced
- Mathematics - Latex  

## How MD works with Web?
******
Origin from  [Markdown](https://daringfireball.net/projects/markdown/)  
Summarized by [Jenny Jing XU](https://www.linkedin.com/in/jenny-jing-xu-a8061342/) in June 19 2020

******

******