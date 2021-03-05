## Here I will put my notes about the Markdown topic from Read02

### What is Markdown?
    Markdown is a way to style text on the web. You control the display of the document; formatting words as bold or italic, adding images, and creating lists are just a few of the things we can do with Markdown. Mostly, Markdown is just regular text with a few non-alphabetic characters thrown in, like # or *.
    
You can use Markdown most places around GitHub:

  - Gists
  - Comments in Issues and Pull Requests
  - Files with the .md or .markdown extension

### here some application, command and syntax that we use in markdown

 - links
    
        [link to Google!](http://google.com)
 - Section links

    You can link directly to a section in a rendered file by hovering over the section heading to expose the link In the below image you will see the shape that i said about:

    ![SectionLink](https://docs.github.com/assets/images/help/repository/readme-links.png) 
    Note: by copying the link which will be on your browser search box and put it on link the page will scroll to this section when you press to the link
 - Relative links
    
    You can define relative links and image paths in your rendered files to help readers navigate to other files in your repository.

    A relative link is a link that is relative to the current file. For example, if you have a README file in root of your repository, and you have another file in docs/CONTRIBUTING.md, the relative link to CONTRIBUTING.md in your README might look like this:

        [Contribution guidelines for this project](docs/CONTRIBUTING.md)
    
 - lists
    Sometimes you want numbered lists:

    1. One
    2. Two
    3. Three

    Sometimes you want bullet points:

    * Start a line with a star
    * Profit!

    Alternatively,

    - Dashes work just as well
    - And if you have sub points, put two spaces before the dash or star:
        - Like this
        - And this
 - images
    ![Image of Yaktocat](https://octodex.github.com/images/yaktocat.png)
 - heading
    # biggest one
    ###### The smallest one
 - code
   ```javascript
    if (isAwesome){
    return true
    }
    ```
 - Inline code
    I think you should use an
    `<addr>` element here instead.
 - Strikethrough
    ~~yaser~~
 - bold
    **yaser**
 - italic
    *yaser*

 - Blockquotes
    As Kanye West said:

    > We're living the future so
    > the present is our past.
- Task Lists
        
    [x] @mentions, #refs, [links](), **formatting**, and <del>tags</del> supported
    
    [x] list syntax required (any unordered or ordered list supported)
    
    [x] this is a complete item
    
    [ ] this is an incomplete item

 - Tables
    First Header | Second Header |
    ------------ | ------------- |
    Content from cell 1 | Content from cell 2 |
    Content in the first column | Content in the second column |