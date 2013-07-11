## Pick Your Own Adventure

* [Instructions](#instructions)
* [Educator Guide](#educator)
* [Basic HTML Tags](#html_tags)
* [Sample App](#sample_app)
* [Additional Links](#additional_links)

### Instructions
<a href='#instructions'/>

1. Start off by asking the kids to think of a setting / plot for their adventure game
2. Download the HTML [template](http://coderdojonyc.s3.amazonaws.com/adventure-game-template.zip) - http://coderdojonyc.s3.amazonaws.com/adventure-game-template.zip
3. Open up the **index.html** file in TextEdit (Mac), NotePad (Windows) or an editor of their choice. [Sublime](http://www.sublimetext.com/) is a good alternative.
4. Now you can being creating your own adventure game!


### Educator Guide
<a href='#educator'/>

Give the kids a piece of paper and tell them to start planning out their adventure game. If they can't come up with an idea, ask them what their favorite vacation spot is. Then ask them to name some things they might find at that location. 

Before you start create a folder somewhere and name it `coderdojo`. Inside it make another folder called `images`.

Your directory structure should look something like this

    /coderdojo
    /coderdojo/images


Now that you've chosen a setting, go on google images and find an image that pertains to the place. Since my game takes place in a haunted house, I'm going to download an image of a haunted house and save that into the images folder I just created.

Next I will create an `index.html` file in the /coderdojo folder. My directory should look something like this

    /coderdojo
    /coderdojo/index.html
    /coderdojo/images/haunted_house.jpg

Open the `index.html` file with a text editor of your choice. We recommend Sublime if you don't have one.

You should be greeted with a blank file. To get started type the following. Don't worry, we'll explain what everything means shortly.

    <html>
        <head>
            <title>Adventure Game</title>
        </head>
        <body>
        
        </body>
    </html>
    
This is the general foundation of every webpage you will be creating. HTML (HyperText Markup Language) is comprised of tags. These tags provide instructions to the computer and tell it how to format the text. 

There are several rules to tags.

Rule #1: All tags are wrapped in < and >.

Example Tags:
    
    <html>
    <b>
    <i>
    <u>
    <p>
    <img>
   
Rule #2: All tags come in pairs.

Example:
    
    <html></html>
    <b></b>
    <i></i>

`<html>` is a start tag. The end tag has a forward slash (/) following the less than (<) symbol. Example end tag: `</html>`

Every HTML page must start with a <html> tag and end with the </html> tag. The <head> tag is where you code to modify your favicon or webpage title. We can also add CSS stylesheets in here, but we'll get more into that later. The <body> tag is where you put code you want to render onto the screen.

Since my adventure game revolves around haunted houses, I'll start off by typing `In the far distant you see a haunted house…` into the body

    <body>
        In the far distance you see a haunted house…
    </body>
    
Now save the page and double click on the index.html file. You should see something like this on browser. Congratulations, you've successfully created your first webpage.

Now we are going to add the image we downloaded earlier onto our website. We'll use the image tag (<img>) to do this.

    <body>
        In the far distance you see a haunted house…
        <img src='/images/haunted_house.jpg'/>
    </body
    
`<img/>` is just a short hand of writing <img></img>. Tags can have attributes. Attributes are modifiers for tags. In this case, the image tag has a modifier `src`, which represents source. You need to tell the image where the image is located. 

Once you have done that, save the page and you should see the image rendered onto the screen.

Now we're going to build out our game a little more by giving the player an option as to what to do after they see the haunted house.

    <body>
        In the far distance you see a haunted house…
        <img src='/images/haunted_house.jpg'/>
        <p>
            Continue Towards The House
            
            Run the Other Direction
        </p>
    </body
    
There we introduced a new tag `<p>`. The <p> tag is the paragraph tag. You may have noticed that `Continue Towards the House` and `Run the Other Direction` are on the same line even though we had line breaks in the markup. If you want two lines in between you can do the following.

    <p>Continue Towards the House</p>
    <p>Run the other Direction</p>

Another alternative is to use the `<br/>` or break tag.

    Continue Towards the House<br/><br/>
    Run the other Direction
    
You will need to use two line break tags if you want an empty line between the sentences.

Now we'll actually need to make the actions actionable. To do this we'll have to wrap the text in anchor tags.

    <body>
        In the far distance you see a haunted house…
        <img src='/images/haunted_house.jpg'/>
        <p>
            <a href='towards.html'>
                Continue Towards The House
            </a>
            
            <a href='other.html'>
                Run the Other Direction
            </a>
        </p>
    </body

The `a` tag has a similar attribute (href or hyperlink reference) to the <img> src attribute. Both attributes require a file path as a value. In this case we are pointing it to two HTML files we are going to create. If we wanted we could also point the <a> tags to some page on the web.

    <body>
        In the far distance you see a haunted house…
        <img src='/images/haunted_house.jpg'/>
        <p>
            <a href='towards.html'>
                Continue Towards The House
            </a>
            
            <a href='http://www.coderdojo.com'>
                Run the Other Direction
            </a>
        </p>
    </body

If you haven't already, create two HTML files, one called `towards.html` and the other called `other.html`.

Your folder structure should look something like this now.

    /coderdojo
    /coderdojo/images/haunted_house.jpg
    /coderdojo/index.html
    /coderdojo/towards.html
    /coderdojo/other.html
    
Okay, now you can build out the towards.html / other.html file in a similar fashion as you did with the index.html page.

*(PLACEHOLDER >> Add CSS / Absolute Positioning Here)*


### HTML Tags
<a href='#html_tags'/>

If you don't know any HTML, that's okay. The only tag you will probably need to know is the **A** or [anchor tag](http://www.w3schools.com/html/html_links.asp). The anchor tag is used to create links. Below are a few examples of links.

```html
<a href='turn_right.html'>Turn Right!</a>
<a href='http://www.coderdojo.com'>Click here to go to CoderDojo!</a>
<a href='http://www.coderdojo.com'>CoderDojo!!!</a>

```

Let's say you wanted to link an image instead, you would just wrap the anchor tag around an [image tag](http://www.w3schools.com/html/html_images.asp).

```html
<a href='page2.html'>
    <img src='http://placehold.it/100/100'/>
</a>
```

* Sample Tags >> http://rickyc.github.io/citizens-school-spring-2012/
* Color Picker >> http://www.colorpicker.com/

### Sample App
<a href='#sample_app'/>

https://coderdojonyc.s3.amazonaws.com/adventure-1/index.html


### Additional Links
<a href='#additional_links'/>

**Playgrounds**

* http://codepen.io
* http://dabblet.com
* http://jsfiddle.net

**HTML Resources**

* http://www.w3schools.com/html/
* https://www.mtholyoke.edu/acad/germ/neh/HTML.html
* http://www.codecademy.com/courses/web-beginner-en-HZA3b?curriculum_id=50579fb998b470000202dc8b

**Other**
* http://neocities.org/ # Free Website Hosting