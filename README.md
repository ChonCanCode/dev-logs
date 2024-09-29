# dev-logs
 
A journal entry for my coding journey.

**2024.07.01**

- Learned the basic of Markdown
- Learned the importance of having a good GitHub profile
- Learned a new term boilerplate code (a piece of code I can use over and over again)

**2024.07.02**
- Time spent: 84 mins
- HTML basic structure completed, ready to move on to CSS
- Learned: `Common Semantic HTML Tags, Word Tags, Elements <input/>, <a>, <span>.`

**2024.07.03**
- Time spent: 40 mins
- Started coding on CSS, learned that I can use website inspection(Q), to highlight each session on the website to show spacing.

**2024.07.04**
- Time spent: 126 mins
- Project-01-google-search: responsive web completed
- Learned how to air my website for free on Netlify!

**2024.07.05**
- Time spent: 40 mins
- Study more on CSS - Flexbox syntax and functionality

**2024.07.08**
- Time spent: 120mins
- Started project-02-website-portfolio
- HTML basic structure completed

**2024.07.09**
- Time spent: 40mins
- Started working on CSS

**2024.07.10**
- Time spent: 120mins
- Learned to use information from GitHub profile for personal info

**2024.07.11**
- Time spent: 50mins
- Putting anchor tags on icons and projects for direction to the relevant page.
- Putting Webiste live

**2024.07.13**
- Time spent: 120mins
- Started project-03-tailwindcss-starter
- Installing tailwindcss via terminal, COOL!

**2024.07.14**
- Time spent: 120mins
- Fixed some issue with loading up the content
- Learned how to open up the config page & adding extra style on it.
- Leanred the basic of using class system to style the page. Skipping coding for CSS. 

**2024.07.15**
- Time spent: 45mins
- Learned `Responsive Classes` 
- Learned how to adjust photo size with `h-, sm:h `
- Learned how to add badge on top of the photos

**2024.07.16**
- Time spent: 30mins
- Leanred how to use custome selector with `@apply directory` to simplify reusable styles.

**2024.07.17**
- Time spent: 120mins
- Finished project-03-tailwindcss-starter

**2024.07.19**
- Time spent: 90mins
- Begin, project-04-reactjs-starter

**2024.07.20**
- Time spent: 120 mins
- Contunie working on reactjs project
- Learned exporting and importing files within the project. 
- Leanred how HTML & JS can work side by side in one single code block in JSX file. 

**2024.07.21**
- Time spent: 120 mins
- Struggle to get me head around understanding logic of taking the input and adding a new element on to the website step by step. 

**2024.07.26**
- Time spent: 60 mins
- Completed, project-04-reactjs-starterProject completed
- Struggle to understand how each step work from beginning to end
- Need to look for a more basic project to learn JS

**2024.07.27**
- Time spent: 30 mins
- Objects and Object Constructors

**2024.07.28**
- Time spent: 30 mins
- Continue - Objects and Object Constructors

**2024.07.29**
- Time spent: 30 mins
- Continue - Objects and Object Constructors

**2024.07.30**
- Time spent: 120 mins
- Continue - Objects and Object Constructors

**2024.08.02**
- Time spent: 120 mins
- Completed - Objects and Object Constructors
- Create a reusable guide for building up 

**2024.08.06**
- Time spent: 120 mins
- Building up a go to page for both HTML & CSS

**2024.08.09**
- Time spent: 240 mins
- HTML & CSS build guide completed, will look a page to build without following online guide. Only with self-guide approach to ensure I can build a page by myself. 

**2024.08.10**
- Time spent: 45 mins
- Finding new project to build, learn how to build from inspecting existing website. 

**2024.08.11**
- Time spent: 120 mins
- Begin, project-05-website-youtube

**2024.08.12**
- Time spent: 60 mins
- Continue, project-05-website-youtube

**2024.08.30**
- Time spent: 190 mins
- Continue, project-05-website-youtube


**2024.09.12**
- Completed, project-05-website-youtube
- Got a better understanding of how to build the entire page from scratch, better usage of border, flex box and layout. Moving forward need to understand how to make website interactive from scratch.

**2024.09.14**
- Begin, beginner-js-project-01-colours.
- Started a very simple tutorial of using JS in website.
- JS "`document.`" it refers to the *Document Object Model (DOM)*, which represents the structure of an HTML or XML document. The `document` object is hte entry point that enables you to interact with and manipulate the content, structure, and style of the HTML document via JS. 
- JS `getElementsByTagName()` is a DOM Method. It is a HTML element retrieval method, as it used to find and retrieve all HTML elements that matach a specific tag name(e.g., `<div>, <p>,<span> `etc).
- In JS a method is simply a funcion that is associated with an object (in this case the `document` object).
- DOM (Document Object Model) - a programming interface (or structure) that represents the HTML or XML document loaded in a web browswer. It allows programs like JS to interact with, manipulate and update the content.
- DOM - Real-Time Representation, when open a webpage, the browswer parses the HTML and builds the DOM. JS can then access and manipulate this DOM to modify the content without reloading the page.
- DOM - Tree-like structure. The root of the tree is the `<html>` element. Other nodes represents the head, body, divs p and img and so on.
- DOM - Nodes. Everything in the DOM is treated as node. Like Element nodes `<div>, <p>, <h1>`. Attribute nodes, id, class, src. Text nodes, the actual text content inside the element.

The DOM representation 
```
Document
 └── <html>
      ├── <head>
      │    └── <title>
      └── <body>
           ├── <h1>
           └── <p>
```

- `index > colours.length-1` the `.length-1` prevent the index goes beyond 5 if it happens purple will appear twice as it has to perfrom the loop again to reset it to red which is 0. A loop base. If the number is 4 the purple will only appear once.

```
function changeColours() {
    let colours = ["red", "blue","orange","yellow","green","purple"];
    
    document.getElementsByTagName("body")[0].
    style.background = colours[index++];

    if(index > colours.length-1)
        index = 0;
}

```

**2024.09.15**
- Begin, beginner-js-project-02-Hex-Colours.
- JS `Math.` is a built-in JS object that provides a variety of mathematical functions nad constants.
- JS `Math.random()` generates a random decimal number between 0 (inclusive) and 1 (exclusive). This means form 0 - 0.999999.
```
function changeColours() {
    let hex_numbers = ["0","1","2","3","4","5","6","7","8","9","A","B","C","D","E","F"];

    let hexcode = '';

    for (let i=0; i < 6 ; i++) {
        let random_index = Math.floor(Math.random() * hex_numbers.length);


        hexcode += hex_numbers[random_index]
    }

    document.getElementById("hex-code").innerHTML = hexcode;
    document.getElementsByTagName("body")[0].style.background = "#" + hexcode;

}

```

**2024.09.18**
- Completed, beginner-js-project-02-Hex-Colours. 
- CSS `animation` property, it conisits of several shorthand properties within the code. It apply elements with animation.
    -  `colourchange` is the name of the animation

```
animation: colourchange 5s infinite alternate;
animation: <animation-name> <animation-duration> <animation-timing-function> <animation-delay> <animation-iteration-count> <animation-direction> <animation-fill-mode> <animation-play-state>;
```

- CSS `@` is at-rule followed by a keyword that dictates the behaviour of the rule. These rules can serve various purposes such as importing other CSS file.
    - `@import` to import an external stylesheet into thecurrent stylesheet.
    - `@media` to apply styles based on certain condition, like screen size or device orientation.
    - `@keyframes` to apply rule specifies the intermediate stages of an animation.
    - `@font-face` to allow custom font to be used in CSS by defining the font source.
    - `@supports` to check if the browser supports a certain CSS feature or property before applying a block of styles.
    - `@charset` to declarethe character encoding of the CSS file.


- JS `.innerHTML` property in JS is used to get or set the HTML content of an element.
- JS `document.getElementByTagName("body")[0]` the `[0]`meaning it will acess the first element within the body element.

```
document.getElementById("Hex-code").innerHTML = hexcode;
document.getElementByTagName("body")[0].style.background = '#' + hexcode

or this

document.getElementsByClassName("hex-colours")[0].style.background = "#" + hexcode;/
```

**2024.09.18**
- Completed, beginner-js-project-03-quote-generator. 
```
function generate(){
    let quotes = {
        "- Jules Renard" : '"The truly free man is the one who can turn down an invitation to dinner without giving an excuse."',
        "- Albert Einstein" : '"Our task must be to free ourselves... by widening our circle of compassion to embrace all living creatures and the whole of nature and its beauty."',
        "- Vera Nazarian" : '"A choir is made up of many voices, including yours and mine. If one by one all go silent then all that will be left are the soloists."',
    }

    let authors = Object.keys(quotes);
    
    let author = authors[Math.floor(Math.random() * authors.length)];

    let quote = quotes[author];
    
    console.log(author)
    console.log(quote)

    document.getElementById("quote").innerHTML = quote;
    document.getElementById("author").innerHTML = author;
}
```

**2024.09.22**
- Begin, beginner-js-project-pass-the-message
- HTML `<label>` element is define a label for an iput element to provide a decscription of the input field it is associated with.
- HTML `for=""` attribute inside the label element tag specifices which input element the label is associated with. The value of the for="" whould match the `id=""` of the corresponding input field.
```
                <label for="messag-input">Enter a message</label>
```
- HTML `<br>` stands for break elementis used to insert a line break in the text. 


- Method 1 `input=""` doesn't work, as it is a local variable that stors the value of the input field(from document.getElementById("message-input").value). However if i change to `document.getElementById("message-input").value = "";` this will work because I directly modify the value ofthe actual input field(the DOM element).

`const input = document.getElementById("message-input").value;` This line fetches the current value of the input field and stores it in the variable input. However, this is ***only a copy of the value*** at the moment the line is executed. It does not reference the input field itself; it just stores the current value as a string.

```
//Method 1

function getMessage() {
    
    const input = document.getElementById("message-input").value

    document.getElementById("message-output").innerHTML = input;

    input="";
}


//Method 2

const messageInput = document.getElementById("message-input")

function getMessage() {
    document.getElementById("message-output").innerHTML = messageInput.value;

    messageInput.value="";
}
```
- beginner-js-project-pass-the-message, completed.

- Need to understand how the following work
```
messageInput.addEventListener("keydown", function(event) {
    if(event.key == "Enter")
    getMessage();

})
```


**2024.09.28**
- beginner-js-project-05-counter
- straight forward JS
```
let count = 0;

function changeCount(num) {
    count += num;

    document.getElementById("count").innerHTML = count
}

```

**2024.09.28**
- beginner-js-project-06-image-carousel
- Made a stupid mistake in HTML "script.css" instead of "script.js"

