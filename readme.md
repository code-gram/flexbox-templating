# website template development using html/html5, css/css3 and flexbox

## Req_001 : Project setup for flexbox app template project

```
- Create index.html, about.html, services.html and contact.html pages in your application folder
- Create ** css ** and ** images ** folder in the application folder.
- Create ** style.css ** file in **css** folder
- Generate basic html scaleton using shortcut technique [Hint: Emmet plugin]
- Link ** style.css ** in the **index.html** in the head section
- Write below code in **style.css** to check, whether style sheet connected with html or not and run the index page

>body{background:red;}

- download flexboxgrid css from the provided location and add flex box grid css file in css folder.
- flexbox grid file location :  http://flexboxgrid.com/
- link **flexboxgrid.css** in the index.html file on top of custom link

```
=============================================================================================================
## Req_002 :  Header Component visualization and Creation

###### Observation for Header Component
```
In the Header component, we have two parts.
1. logo section [taking 2 cols out of 12 col grid]
2. navigation section [taking 10 cols out of 12 col grid]

Below are some of the observations.

- Logo and navigation will be wrapped in a container [container is covering 80% area in the centre of the screen]

- Both logo and navigation is wrapped inside a row.

```
###### Instructions for Header Component Creation
```
- Create **header** tag with main-header id and put some //TODO : Header Section text for testing. check on browser for changes. 
- Create a div inside header tag with **container** class, and put the same placeholder text and test application. 
- Create a div inside **container** div and add class attribute as **row**.
- Inside row div, Create two divs with empty class attribute. First for logo and second for navigation.
- Logo will be displayed in **h2** tag. In which **Flex** word is styled differently. Keep flex word in <span class="primary-text">Flex</span>. **primary-text** style will be provided later. 
- Create div section with empty class attribute inside a row,  below the logo div.
- Create a **ul** with 4 **li** as given below. 

<div class="">
        <nav id="navbar">
            <ul>
                <li><a href="index.html">Home</a></li>
                <li><a href="about.html">About</a></li>
                <li><a href="services.html">Services</a></li>
                <li><a href="contact.html">Contact</a></li>
            </ul>
        </nav>
</div>

- Now Test your application
```

###### Arranging the logo on left side and navigation to right side.
- We need to shift the logo on left side and navigation to the right side. 
- For this very first we need to visualize the whole row behaviour.
    - for the extra small screen, logo will be displayed in center. for mobile, tablet and desktop view, logo will be displayed in the end, covering the 2 cols, out of 12.
    - For the extra small screen, navigation will be on right side, and will be covering the 10 cols out of 12. Remaining properties will be commonly applied. 
    
- Refer the Slide no 19 in training for more detail. 

###### Keeping the header in the center of the screen.
- At present header is arranged on the screen as per default setting. 
- Now it should be displayed in the center of the screen
- Hint: Screen's margin and padding should be nutralized, and container's margin should be auto adjustable.

=============================================================================================================

## Req_003 :  SHOWCASE Section

###### Instructions to create showcase section
```
- The whole showcase section, including image, tagline and info section will be under **section** tag.
- Inside section, use container, because showcase section is displayed in the center of the screen.
- There will be a row inside container, and row will be responsible for the content arrangement according to different screen sizes. 
    - extra small screen :  center
    - small screen : center
    - tablet screen: center
    - desktop screen: center
    
    - extra small screen :  middle of the section
    - small screen : middle of the section
    - tablet screen: center of the section
    - desktop screen: center of the section
- Inside the row, a column division will be there covering 7 cols in case of large screen, otherwise 10 cols for all out of 12 cols. This division will also have showcase-content section.
- Inside the showcase-content division, put one **h1** tag to display Tag line and **p** tag for info part.
        
```

=============================================================================================================

## Req_004 :  FEATURES Section

###### Instructions to create Features section
```
- The whole Features section, including heading, paragraph and two other sections with icon, heading and paragraph will be under **section** tag.
- Inside section, use container, because features section is displayed in the center of the screen.
- There will be a row inside container, and row will be responsible for the content arrangement according to different screen sizes. 
    - extra small screen :  center
    - small screen : center
    - tablet screen: center
    - desktop screen: center
- Inside the row, Create col division in which main heading and paragraph will always cover 12 cols and will be in center of the screen irrespective to the screen sizes.
- Below the main heading and paragraph, add division for row, that will display the content in the center of the screen, irrespecitive to the screen size.
- inside row division, add col division that will be displaying content in the 12 cols only for extra small screen, otherwise in all screen sizes this will display the 4 cols.
- for using icon add below code just below the custom css on top of the page inside head section. 
    <script src="https://kit.fontawesome.com/a4990f058a.js" crossorigin="anonymous"></script>
- Use below icons code
- 1st Div :  
    icon : <i class="fa fa-dashboard"></i><br/>
    heading : Fully optimized
    Paragraph : some lorem text
- 2nd Div :  
    icon : <i class="fa fa-question-circle-o"></i><br/>
    heading : Free Support
    Paragraph : some lorem text
- 3rd Div :  
    icon : <i class="fa fa-rocket"></i><br/>
    heading : Free Upgrade
    Paragraph : some lorem text
- 4rd Div :  
    icon : <i class="fa fa-line-chart"></i><br/>
    heading : Uptime Gurantee
    Paragraph : some lorem text
- 5th Div :  
    icon : <i class="fa fa-users"></i><br/>
    heading : Multi User
    Paragraph : some lorem text
- 6th Div :  
    icon : <i class="fa fa-plug"></i><br/>
    heading : Plug & Play
    Paragraph : some lorem text
        
```

=============================================================================================================

## Req_005 :  INFO Component Creation

###### Observation for info Component
```
- Separate info section
- The whole part is displayed in center of the screen
- Two informations are displyed taking equal part of the section. one is image, second is core feature listing.

```

###### Creating info Component
```
- Create a section with info id
- Create a div inside info section with container class
- Create a div inside container with row class
    - center-xs center-sm center-md center-lg middle-xs middle-sm middle-md middle-lg
- Create a div inside row for image section, it will be covering only 6 cols for each screen sizes, except extra small
    - col-xs-12 col-sm-6 col-md-6 col-lg-6
- add imphone image from the provided location inside first col section.
- Create another div inside row for Core Feature listing, it will be covering remaining 6 cols for each screen size, except extra small
    - col-xs-12 col-sm-6 col-md-6 col-lg-6
- Create core Feature and ul list with check mark icon.
    - <i class="fa fa-check"></i>

```

=============================================================================================================

## Req_006 :  COMPANY Component Creation

###### Creating Company Component
```
- Create a section with company id
- Create a div inside company section with container class
- Create a div inside container with row class
    - center-xs center-sm center-md center-lg
- Create a div inside row for contact us detail which includes: which includes contact us header, phone no with icon, email with icon, address with map icon.
    - col-xs-12 col-sm-4 col-md-4 col-lg-4
    -<i class="fa fa-phone"></i>
    -<i class="fa fa-envelope"></i>
    -<i class="fa fa-map"></i>
    
- Create a div inside row for About us detail which includes: which includes about us header and paragraph.
- Create a div inside row for Newsletter detail which includes: which includes Newsletter header, paragraph and form

```

=============================================================================================================

## Req_007 :  Footer Component Creation
###### Creating Footer Component
```
- Create footer tag with main-footer id
- Create division inside footer with container class
- Create division inside container with row class and use below classes.
    center-xs center-sm center-md center-lg
- Create a division inside row and use below classes.
    col-xs-12 col-sm-12 col-md-12 col-lg-12
- now inside the above division create **p** tag, that should contain footer text

```

=============================================================================================================

## Req_008 :  Cosmatics of the site |Navigation
###### Adding effects on site. Instructions for decorating Header.

- Very first the whole site will have a universal font-family, font-size and there will be a line-height of 1.5 em. so add below properties in the body section and see the changes. 
- As a best practice you should add comment over each style element. Follow the syntax from body

```
/* BODY */
body{
    font-family: 'Open-sans', sans-serif;
    font-size: 17px;
    line-height:1.5em;
}
```
- All the images will be having a width of 100% of its container. We have an image of iphone. Add below css and see the effect on your browser. 
```
/* IMG */
img{
    width:100%;
}
```
- As you see in the final output of the header, half of the logo part is styled differently. Add below style in the style.css, under the section of /* COMMONS */. All the elements in index.html having 'primary-text' as class, will be refelected with below changes. 
```
/* COMMON CLASSES */
.primary-text{
    color:#56a79a;
}

.primary-background{
    background:#56a79a;
}
```

- There is a border in the bottom of the header pannel. Add below property and see the changes. 

```
/* MAIN-HEADER */

#main-header{
    border-bottom: 1px solid #56a79a;
}
```
- In the Navigation, each option is in upper case. Add below style to make it upper case. 

```
/* NAVBAR */

#navbar {
    text-transform: uppercase;
}
```
- In the navbar all li items are displayed in one line, without any style and each item having right side padding of 20px. Add the respective style to below style.

```
#navbar li {

}
```

- In the navbar all the anchor tags are displayed without link effect, and having a color as #888. make appropriate changes in the below style.

```
#navbar a{

}
```
- Current navigation item and when user hover on that item is displayed in different style. below is the code for your reference.

```
#navbar li.current a, #navbar a:hover{
    color:#56a79a;
    border-bottom: 3px solid #56a79a;
    padding-bottom: 3px;
}
```

=============================================================================================================

## Req_009 :  Cosmatics of the site | Showcase
###### Instructions for decorating Showcase section.

- showcase section has a background image stretched to whole screen. having border-bottom as 1px solid #56a79a and having a margin in bottom as 30px; follow below code and see the effect. 

```
#showcase{
    background: url('../images/showcase.jpg') no-repeat center center;
    border-bottom: 1px solid #56a79a;
    margin-bottom: 30px;
}
```

- When you add the above code and check your browser, you will get image in full width, but in the final output, this coveres the whole page. We have one row class inside showcase section. we can add height of 600px to this row. Add below code and see the effect. 

```
#showcase .row{
    height: 600px;
}
```

- We have a "Welcome to flexbox demo" heading in showcase. We want to give it a different style. 
    - font-size as 40px
    - margin 0 from all sides.
    - padding from bottom as 20px
 Add the style in below style element. 
```
#showcase h1{
   
}
```

- Below the heading we have a paragraph, which should have color code as #ccc and margin 0 from all sides. Add appropriate style in the below style element.
```
#showcase p{
    
}
```
- we hava showcase-content class inside the showcase section. This class we had added for rounded shape on which showcase content is displayed. Add below rules in the provided style element.
    - background color : #333
    - color:#fff
    - radius from all corners :  90px
    - padding from all sides: 40px
    - transparency level : 0.9

```
#showcase .showcase-content{
    
}
```
=============================================================================================================
## Req_010 :  Cosmatics of the site | Feature
###### Instructions for decorating Feature section.

-  h2 header of features section will have below style rule. 
    - font-size of 35px
    - margin from all side as 0
    - padding from bottom as 10px
    Add all the rules in the below style element.   

```
/* FEATURES */
#features h2{
   
}
```
- All the paragraphs in features section will have below style rules. 
    - color: #888;
    - margin from all side as 0
    - margin from bottom as 40px;
    Add above rule in the below style element
```
#features p{
    
}
```

- All icons in features section will have below style rules. 
    - font-size :  60px
    - color : #56a79a 
    Add above rule in the below style element
```
#features .fa{

}
```

=============================================================================================================
## Req_011 :  Cosmatics of the site | Info
###### Instructions for decorating Info section.

- info section has background with image and forground color as #fff. Add below rule in the provided style element. 
    - background - #333 url('../images/info-bg.jpg') no-repeat
    - color: #fff
```
/* INFO */
#info{
   
}
```

- for h2 header of info add below rules in the provided style element. 
    - font-size: 35px
    - margin:0
    - padding-bottom: 10px

```
#info h2{
    
}
```

- for unordered list of info section below are the style rules. 
    - list-style :  none
    - padding: 0

```
#info ul{
   
}
```

- each li element will have below style rule for info section only. 
    - line-height: 2em
    - font-size:20px

```
#info li{
    
}
```

=============================================================================================================
## Req_012 :  Cosmatics of the site | Company
###### Instructions for decorating Company section.

- Company section will have below style rules.
    - background: #333
    - color: #fff
    - padding : 10px 0
    Add above rules in the provided style element. 
```
/* COMPANY */
#company{
    
}
```

- All h4 headings should have below rules. 
    - text-transform: uppercase;
    - margin-bottom: 0;
    Add below rule in the provides style element. 
```
#company h4{
    
}
```
- unordered list under company section will have below rules. 
    - padding: 0;
    - list-style: none;
    - line-height: 2em;
    Add below rule in the provides style element.  
```
#company ul{
    
}
```

- Input box of company section will have below rules.
    - padding:7px;
  Add below rule in the provides style element.  
```
#company input[type="text"]{
    
}
```

- in the newsletter section of company we have a button. on button below style rule will be applied. 
    - background:#222;
    - padding:10px;
    - color:#fff;
    - border:0;
    Add below rule in the provides style element.
```
#company button{
 
}
```
=============================================================================================================
## Req_013 :  Cosmatics of the site | Footer
###### Instructions for decorating Footer section.

- Footer section we keep very simple. below is the style rule, that will be applied on footer section. 
    - background:#56a79a;
    - color:#fff;
```
/* FOOTER */
#main-footer{
    
}
```

=============================================================================================================
## Req_014 :  Other template pages Creation
###### Instructions for creating and decorating other template pages. 

- Copy the complete code of index.html page.
- Create about.html, services.html and contact.html page and paste the code copied from index.html page. 
- Make the changes in the title of each page as below.
    <title>Flexbox | Contact</title> for contact.html page. Same for other two pages as well. 
- Make the changes in the Navigation to make current class as shown below. 
    <li class="current"><a href="contact.html">Contact</a></li>. Same for other two pages as well. 

=============================================================================================================
## Req_015 :  Other template pages Creation | about.html
###### Instructions for creating and decorating about.html page -  subheading section

- About us will be displayed in the subheading. 
- Create a section with subheading id
- Create a container inside subheading id
- Create a row inside container
- Create a division inside row, which will be displaying the content in whole 12 cols for all screen sizes. 
- Create one h1 heading inside division, that should display About us text

- Styling for the subheading part
    - background: #333
    - color :  #fff

###### Instructions for creating and decorating about.html page -  page section

- Create a section with page id and about class
- Create container divisio inside page
- Create row division inside container division. this row division will be displaying the content in the center of the screen despite of any screen size.
- Create a division inside row division, this will display the heading and paragraph in the 12 cols dispite of any screen size.
- Use below code for your heading and paragraph. 
    <h2><span class="primary-text">Who</span> We Are</h2>
    <p>lorem text</p>
    <hr>
    
- Styling for the page id
    - margin-bottom:40px

=============================================================================================================
## Req_016 :  Other template pages Creation | service.html
###### Instructions for creating and decorating service.html page
- Subheader with different message will be as it is
- Create a section with page id and services class
- Create a container inside page section
- Create a row inside container, that should display all the content in the center of the screen despite of any screen size.
- Create a division inside the row, which will be displaying content in 12 cols, despite of any screen size
- Inside the above division, there will be one heading, and unordered list with three list items. 
    Header will be as below
    <h2><span class="primary-text">See</span> What We Offer</h2>
- Each list item will be displaying the h3 heading and paragraph.

- Styling for the services section

- Add below rules in the provided style element
    - list-style: none;
    - padding: 10px;

```
.services ul li{
    
}
```
- Add below style for the nth-child(odd) of list item in the provided style element.
     -background:#333;
     -color:#fff;

```
.services ul li:nth-child(odd){
   
}
```
- Add below style for the nth-child(even) of list item in the provided style element.
    -background:#56a79a;
    -color:#fff;
```
.services ul li:nth-child(even){
    
}
```

=============================================================================================================
## Req_017 :  Other template pages Creation | contact.html
###### Instructions for creating and decorating contact.html page

- Subheader with different message will be as it is
- Create a section with page id and contact class
- Create container division inside contact
- Create a row inside container division, this will be displaying the content in the center of the screen, despite of any screen size.
- Create a division inside of row, which will be covering the entire 12 col grid.
- Inside the division display the below information
     <h2><span class="primary-text">Get</span> In Touch</h2>
     <p>Please use this form to contact us.</p>
- Inside heading, contact form need to be displayed with below detail 
    - Name
    - Email
    - Message
    - Submit button
    
- Styling for contact page
- Add below style for form in the provided style element
    - background: #333;
    - color:#fff;
    - padding: 20px;
    - border-radius: 20px;
```
.contact form{
    
}
```

- Add below style for text boxes, style element is provided. 
    - width: 50%;
    - height: 40px;
    - border: 0 none;
    - border-radius: 30px;
    - margin-bottom: 30px;
    - padding-left: 10px;
```
.contact form input[type="text"]{
    
}
```
- Add below style for the textarea, style element is provided.
    - width:50%;
    - height:100px;
    - padding-left: 10px;
```
.contact form textarea{
    
}
```
- Add below style for the button in the form. 
    - width: 50%;
    - padding: 10px 0;
    - border: 0;
    - background: #56a79a;
    - color:#fff;
    - border-radius: 20px;
```
.contact form button{
   
}
```
- Add below style for labels
```
.contact form label{
    text-transform: uppercase;
}
```


=============================================================================================================
                =====     =   =        =       =    =    =   =     ===
                  =       =___=       = =      = =  =    = =       = =  
                  =       =   =      = = =     =  = =    =   =   = =
                  =       =   =     =     =    =    =    =       === 
===========================================================================================================
