## Pick Your Own Adventure

* [Instructions/Setup](#instructions)
* [Educator Guide](#educator)
* [Basic HTML Tags](#html_tags)
* [Sample App](#sample_app)
* [Additional Links](#additional_links)

### Instructions / Setup
<a href='#instructions'/>

1. Open up the browser to Mozilla Thimble (https://thimble.webmaker.org/)
2. Create an account on Neocities.org (https://neocities.org/)


### Educator Guide
<a href='#educator'/>

Give the kids a piece of paper and tell them to start planning out their adventure game. If a worksheet is available, use the provided worksheet instead. If they can't come up with an idea, ask them what their favorite vacation spot is. Then ask them to name some things they might find at that location. Be creative!

Once you have opened the browser to Mozilla Thimble, delete everything on the left hand side (Editor View). The boiler plate code will cause unnecessary confusion.

Tell them to write some text into the editor. On the right hand side the written text should magically start to appear. Explain to them that as they write code on the left hand side, the website will start to appear on the right side.

Let's teach them about tags! There are several rules to tags.

Rule #1: All tags are wrapped in < and >.

Example Tags:
    
    <b>
    <i>
    <u>
    <p>
    <h1>
    <img>
   
Rule #2: All tags come in pairs.

Example:
    
    <b></b>
    <i></i>

`<b>` is a start tag. The end tag has a forward slash (/) following the less than (<) symbol. Example end tag: `</b>`

Since my adventure game revolves around haunted houses, I'll start off by typing `In the far distant you see a haunted house…`

    In the far distance you see a haunted house…
    

Now we're going to bold the text. Let's wrap the text in a `<b>` tag.

    <b>
        In the far distance you see a haunted house…
    </b>


If we wanted to italicize the word `haunted`, it would look like the following.

    <b>
        In the far distance you see a <i>haunted</i> house…
    </b>

Now let's underline `haunted house`.

    <b>
        In the far distance you see a <u><i>haunted</i> house</u>…
    </b>

Great! The adventure game is starting to form. Try to play around with a few other tags, such as `<h1>`, `<p>`, `<center>`.

Now it's time to add an image! Let's go to google and find a haunted house. Right click and copy the URL of the image. To add an image, we'd type the following.

    <b>
        In the far distance you see a <u><i>haunted</i> house</u>…
        <img src='http://someurl.com/hauntedhouse.jpg'/>
    </b>


`<img/>` is just a short hand of writing <img></img>. Tags can have attributes. Attributes are modifiers for tags. In this case, the image tag has a modifier `src`, which represents source. You need to tell the image where the image is located. 

Now we're going to build out our game a little more by giving the player an option as to what to do after they see the haunted house.

    <b>
        In the far distance you see a <u><i>haunted</i> house</u>…
        <img src='http://someurl.com/hauntedhouse.jpg'/>
        <p>
            Continue Towards The House
            
            Run the Other Direction
        </p>
    </b>
    
There we introduced a new tag `<p>`. The <p> tag is the paragraph tag. You may have noticed that `Continue Towards the House` and `Run the Other Direction` are on the same line even though we had line breaks in the markup. If you want two lines in between you can do the following.

    <p>Continue Towards the House</p>
    <p>Run the other Direction</p>

Another alternative is to use the `<br/>` or break tag.

    Continue Towards the House<br/><br/>
    Run the other Direction
    
You will need to use two line break tags if you want an empty line between the sentences.

Now we'll actually need to make the actions actionable. To do this we'll have to wrap the text in anchor tags.

    <b>
        In the far distance you see a <u><i>haunted</i> house</u>…
        <img src='http://someurl.com/hauntedhouse.jpg'/>
        <p>
            <a href='towards.html'>
                Continue Towards The House
            </a>
            
            <a href='other.html'>
                Run the Other Direction
            </a>
        </p>
    </b>

The `a` tag has a similar attribute (href or hyperlink reference) to the <img> src attribute. Both attributes require a file path as a value. In this case we are pointing it to two HTML files we are going to create. If we wanted we could also point the <a> tags to some page on the web.

    <b>
        In the far distance you see a <u><i>haunted</i> house</u>…
        <img src='http://someurl.com/hauntedhouse.jpg'/>
        <p>
            <a href='towards.html'>
                Continue Towards The House
            </a>
            
            <a href='http://www.coderdojonyc.org'>
                Run the Other Direction
            </a>
        </p>
    </b>

Now we're ready to move on to Neocities. If you didn't create an account earlier, please do so now. Click on the `dashboard` (https://neocities.org/dashboard) and you should see an `index.html` file. Hover your mouse over it and click edit. Now copy your code from Mozilla Thimble and paste it into the `index.html` file on Neocities. Make sure you get rid of all the existing content first. Now hit the `Save Changes` button at the bottom of the page.

Now go back to the dashboard and hover your mouse over `index.html`, click anywhere on it except for the edit button. You should see your webpage open up. Now let's go back to the dashboard and click the `New Page` button. Let's create two files, name one `towards` and the other `other`. 

Your folder structure should look something like this now.

    /index.html
    /towards.html
    /other.html

There may be other files in the directory and it's okay! Now let's code the towards.html / other.html file in a similar fashion as you did with the index.html page.

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