# FrontEndCourses

Learning HTML, CSS, Java Script

# All HTML elements can have attributes

        * The href attribute of <a> specifies the URL of the page the link goes to
        * The src attribute of <img> specifies the path to the image to be displayed
        * The width and height attributes of <img> provide size information for images
        * The alt attribute of <img> provides an alternate text for an image
        * The style attribute is used to add styles to an element, such as color, font, size, and more
        * The lang attribute of the <html> tag declares the language of the Web page
        * The title attribute defines some extra information about an element
        * By default, links will appear as follows in all browsers:
            * An unvisited link is underlined and blue
            * A visited link is underlined and purple
            * An active link is underlined and red 

# HTML Links - The target Attribute

    By default, the linked page will be displayed in the current browser window. To change this, you must specify another target for the link.
    
    The target attribute specifies where to open the linked document.
    
    The target attribute can have one of the following values:
        1. _self - Default. Opens the document in the same window/tab as it was clicked
        2. _blank - Opens the document in a new window or tab
        3. _parent - Opens the document in the parent frame
        4. _top - Opens the document in the full body of the window

# Link to an Email Address

    Use mailto: inside the href attribute to create a link that opens the user's email program (to let them send a new email):

# hr tag

    The <hr> tag defines a thematic break in an HTML page, and is most often displayed as a horizontal rule.

# Formatting elements to display special types of text

            <b> - Bold text
            <strong> - Important text
            <i> - Italic text
            <em> - Emphasized text
            <mark> - Marked text
            <small> - Smaller text
            <del> - Deleted text
            <ins> - Inserted text
            <sub> - Subscript text
            <sup> - Superscript text

# pre

    * The HTML <pre> element defines preformatted text.
    * The text inside a <pre> element is displayed in a fixed-width font (usually Courier), and it preserves both spaces and line breaks

# HTML RGB and RGBA Colors

    * An RGB color value represents RED, GREEN, and BLUE light sources.
    * An RGBA color value is an extension of RGB with an Alpha channel (opacity).
    **_rgb(red, green, blue)_**
        Each parameter (red, green, and blue) defines the intensity of the color with a value between 0 and 255.
        This means that there are 256 x 256 x 256 = 16777216 possible colors!
        1. rgb(255, 0, 0) is displayed as red, because red is set to its highest value (255), and the other two (green and blue) are set to 0.
        2. rgb(0, 255, 0) is displayed as green, because green is set to its highest value (255), and the other two (red and blue) are set to 0.
        3. rgb(0, 255, 0) is displayed as blue, because blue is set to its highest value (255), and the other two (red and green) are set to 0.
        4. To display black, set all color parameters to 0, like this: rgb(0, 0, 0).
        5. To display white, set all color parameters to 255, like this: rgb(255, 255, 255).
    _**rgba(red, green, blue, alpha)**_
        The alpha parameter is a number between 0.0 (fully transparent) and 1.0 (not transparent at all)

# HTML HEX Colors

    * A hexadecimal color is specified with: #RRGGBB, where the RR (red), GG (green) and BB (blue) hexadecimal integers specify the components of the color.
    _**#rrggbb**_
        * Where rr (red), gg (green) and bb (blue) are hexadecimal values between 00 and ff (same as decimal 0-255).
        * #ff0000 is displayed as red, because red is set to its highest value (ff), and the other two (green and blue) are set to 00.
        * #00ff00 is displayed as green, because green is set to its highest value (ff), and the other two (red and blue) are set to 00.
        * #0000ff is displayed as blue, because blue is set to its highest value (ff), and the other two (red and green) are set to 00.
        * To display black, set all color parameters to 00, like this: #000000.
        * To display white, set all color parameters to ff, like this: #ffffff. 

# HTML Images Syntax

    * The HTML <img> tag is used to embed an image in a web page.
    * Images are not technically inserted into a web page; images are linked to web pages. The <img> tag creates a holding space for the referenced image.
    * The <img> tag is empty, it contains attributes only, and does not have a closing tag.
    * The <img> tag has two required attributes:
        src - Specifies the path to the image
        alt - Specifies an alternate text for the image
    * If you have your images in a sub-folder, you must include the folder name in the src attribute:
        Example
            <img src="/images/html5.gif" alt="HTML5 Icon" style="width:128px;height:128px;">
    * Some web sites point to an image on another server.
    * To point to an image on another server, you must specify an absolute (full) URL in the src attribute:
        Example
            <img src="https://www.w3schools.com/images/w3schools_green.jpg" alt="W3Schools.com">
    * To use an image as a link, put the <img> tag inside the <a> tag:
        Example
            <a href="default.asp">
                <img src="smiley.gif" alt="HTML tutorial" style="width:42px;height:42px;"></a>

### Common Image Formats

        Here are the most common image file types, which are supported in all browsers (Chrome, Edge, Firefox, Safari, Opera):
    Abbreviation - File Format - File Extension
        APNG - Animated Portable Network Graphics - .apng
        GIF - Graphics Interchange Format - .gif
        ICO - Microsoft Icon - .ico, .cur
        JPEG - Joint Photographic Expert Group image - 
        .jpg, .jpeg, .jfif, .pjpeg, .pjp
        PNG - Portable Network Graphics - .png
        SVG - Scalable Vector Graphics - .svg

# HTML Image maps

    Use the HTML <map> element to define an image map
    Use the HTML <area> element to define the clickable areas in the image map
    Use the HTML usemap attribute of the <img> element to point to an image map
    <picture> - Defines a container for multiple image resources

# HTML Table Tags

    <table> ->Defines a table
    <th> ->Defines a header cell in a table
    <tr> ->Defines a row in a table
    <td> ->Defines a cell in a table
    <caption> ->Defines a table caption
    <colgroup> ->Specifies a group of one or more columns in a table for formatting
    <col> ->Specifies column properties for each column within a <colgroup> element
    <thead> ->Groups the header content in a table
    <tbody> ->Groups the body content in a table
    <tfoot> ->Groups the footer content in a table

    * To add a border, use the CSS border property on table, th, and td elements
    * To avoid having double borders like in the example above, set the CSS border-collapse property to collapse.
    * With the border-radius property, the borders get rounded corners
    * With the border-style property, you can set the appearance of the border.
    * The following values are allowed:
        1.dotted
        2.dashed
        3.solid
        4.double
        5.groove
        6.ridge
        7.inset
        8.outset
        9.none
        10.hidden  

## Vertical Table Headers

    To use the first column as table headers, define the first cell in each row as a <th> element:
        <table>
            <tr>
                <th>Firstname</th>
                <td>Sekhar</td>
                <td>Malathi</td>
            </tr>
            <tr>
                <th>Lastname</th>
                <td>P.T.</td>
                <td>S</td>
            </tr>
            <tr>
                <th>Age</th>
                <td>94</td>
                <td>50</td>
            </tr>
        </table>

# HTML List Tags

    <ul> -> Defines an unordered list
    <ol> -> Defines an ordered list
    <li> -> Defines a list item
    <dl> -> Defines a description list
    <dt> -> Defines a term in a description list
    <dd> -> Describes the term in a description list

    * Unordered List : The CSS list-style-type property is used to define the style of the list item marker. It can have one of the following values:
        1. disc -> Sets the list item marker to a bullet (default)
        2. circle ->Sets the list item marker to a circle
        3. square -> Sets the list item marker to a square
        4. none -> The list items will not be marked
    
    * Ordered List : The type attribute of the <ol> tag, defines the type of the list item marker:
        1. type="1" -> The list items will be numbered with numbers (default)
        2. type="A" -> The list items will be numbered with uppercase letters
        3. type="a" -> The list items will be numbered with lowercase letters
        4. type="I" -> The list items will be numbered with uppercase roman numbers
        5. type="i" -> The list items will be numbered with lowercase roman numbers

# HTML class Attribute
    * The class attribute is often used to point to a class name in a style sheet. It can also be used by a JavaScript to access and manipulate elements with the specific class name.
    * Classes are used by CSS and JavaScript to select and access specific elements
    * The class attribute can be used on any HTML element
    * The class name is case sensitive
    * Different HTML elements can point to the same class name
    * JavaScript can access elements with a specific class name with the getElementsByClassName() method

# HTML id Attribute
    * The id attribute is used to specify a unique id for an HTML element
    * The value of the id attribute must be unique within the HTML document
    * The id attribute is used by CSS and JavaScript to style/select a specific element
    * The value of the id attribute is case sensitive
    * The id attribute is also used to create HTML bookmarks
    * JavaScript can access an element with a specific id with the getElementById() method.

# The HTML script Tag
    * The HTML <script> tag is used to define a client-side script (JavaScript).
    * The <script> element either contains script statements, or it points to an external script file through the src attribute.
    * Common uses for JavaScript are image manipulation, form validation, and dynamic changes of content.
    * To select an HTML element, JavaScript most often uses the document.getElementById() method.   
# The HTML meta Element
    * The <meta> element is typically used to specify the character set, page description, keywords, author of the document, and viewport settings.
    * The metadata will not be displayed on the page, but is used by browsers (how to display content or reload page), by search engines (keywords), and other web services.

