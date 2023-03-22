# Your Project Title

## Technology Used 

| Technology Used         | Resource URL           | 
| ------------- |:-------------:| 
| HTML    | [https://developer.mozilla.org/en-US/docs/Web/HTML](https://developer.mozilla.org/en-US/docs/Web/HTML) | 
| CSS     | [https://developer.mozilla.org/en-US/docs/Web/CSS](https://developer.mozilla.org/en-US/docs/Web/CSS)      |   
| Git | [https://git-scm.com/](https://git-scm.com/)     |    

## Description 

This repo stores the assets and information for the Horiseon home webpage. In the webpage, we can see information such as what services the company provides, the importance of such services, along with the benefits of working with the company.

Originally, the webpage, along with its corresponding stylesheet, was written using a lot of non-semantic coding. Because of that, it used a lot of duplicate code in both the style.css file and the index.html file.

Through changing the div tags in index.html to more readable semantic tags along with consolidating code in the stylesheet, the webpage is able to maintain the same functionality and the underlying code is now much more readable than before.

![Site Landing Page Gif](./assets/images/websitedemo.gif)

## Table of Contents

* [Code Refactor Example](#code-refactor-example)
* [Installation](#installation)
* [Usage](#usage)
* [Learning Points](#learning-points)
* [Author Info](#author-info)
* [License](#license)

## Code Refactor Example

This is one example of the refactoring I did for this website.

As we can see, I changed the first div into a header element so it follows proper semantic coding etiquette, the second div into a nav element, and changed the seo class into an seo id since it is only being called once in the Horiseon website.


```html
<div class="header">
        <h1>Hori<span class="seo">seo</span>n</h1>
        <div>
            <ul>
                <li>
                    <a href="#search-engine-optimization">Search Engine Optimization</a>
                </li>
                <li>
                    <a href="#online-reputation-management">Online Reputation Management</a>
                </li>
                <li>
                    <a href="#social-media-marketing">Social Media Marketing</a>
                </li>
            </ul>
        </div>
    </div>
```

Converting the above non-semantic div with the class of 'header' to an appropriate [<header> semantic element](https://www.w3schools.com/html/html5_semantic_elements.asp). 

```html
    <header>
        <h1>Hori<span id="seo">seo</span>n</h1>
        <nav>
            <ul>
                <li>
                    <a href="#search-engine-optimization">Search Engine Optimization</a>
                </li>
                <li>
                    <a href="#online-reputation-management">Online Reputation Management</a>
                </li>
                <li>
                    <a href="#social-media-marketing">Social Media Marketing</a>
                </li>
            </ul>
        </nav>
    </header>

```

## Installation

If you'd like to install the webpage on your local machine to checkout, please simply clone the github responsitory or download it on to your computer. Then, open the index.html file in your browser.

Optionally, you can also open the webpage in your browser by clicking on this link: [Horiseon Home Page](https://daevidvo.github.io/HTML_refactoring/)

## Usage 

To use the webpage, scroll down to read the information or use the navigation bar and select the section that you'd like to jump to.

## Learning Points 

Through competing this exercise and refactoring the Horiseon webpage, I was able to learn more about semantic HTML elements along with how to consolidate code so that my work doesn't look as messy and sporadic.

More specific examples of refactoring would be changing div tags to semantic tags that describe their proper function such as header and nav.

Another very important aspect of web development that I learned is reverse-engineering someone else's website. By looking at the code, figuring out which portions of the site does what, and how it relates to the stylesheet, I got to understand what it's like to break down already existing code into more managable and digestable portions.

## Author Info


### David Vo

* [LinkedIn](https://www.linkedin.com/in/daevidvo)
* [Github](https://www.github.com/daevidvo)


## License

MIT License

Copyright (c) 2023 daevidvo

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

