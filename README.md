# Data Institute 2019
For students of https://projects.propublica.org/graphics/ida-propublica-data-institute

Here are all of the materials we used to teach the 2019 Data Institute: slides, exercises, links, and homework. This is not an online course and doesn’t have all the context or instruction to be a standalone class.

Want to use our slides? Our teaching materials fall under the [same Creative Commons license](https://creativecommons.org/licenses/by-nc-nd/3.0/us/) we use across our site. [Get more details here.](https://www.propublica.org/steal-our-stories/)

# Curriculum

## Table of Contents
Click to jump directly to:
- [Install Party](#welcome-reception--install-party)

Week 1:
- [Day 1: Intro to Data Journalism, Spreadsheets, Best Practices](#day-1)
- [Day 2: Evaluating data, Open Refine, Analyzing One Variable](#day-2)
- [Day 3: Intro to Mapping, Common Calculations in News, Analyzing Two Variables, Statistics](#day-3)
- [Day 4: Intro to Code, How Websites Work, HTML, CSS](#day-4)
- [Day 5: Intro to Design, Type, Layout & Color, Making a Webpage with Github](#day-5)


Week 2:
- [Day 6: Javascript, JQuery](#day-6)
- [Day 7: Visualizing Data, Charts and Maps](#day-7)
- [Day 8: Web Scraping, Fundamentals of Programming](#day-8)
- [Day 9: Even More Web Scraping](#day-9)
- [Day 10: Final Presentations](#day-10)

## Welcome Reception & Install Party

**ACCOUNTS**
<ul>
  <li><a href="https://github.com/join?source=header-home">Github.com</a><br>(Make sure to confirm your e-mail address)</li>
  <li><a href="https://accounts.google.com/SignUp?service=wise&amp;continue=https%3A%2F%2Fdrive.google.com%2F%23&amp;ltmpl=drive">Google.com</a></li>
  <li><a href="https://app.datawrapper.de/signin">Datawrapper</a></li>
</ul>

**SOFTWARE**
- <a href="https://www.google.com/chrome/browser/desktop/">Google Chrome</a>
- Slack (<a href="https://itunes.apple.com/app/slack/id803453959?ls=1&amp;mt=12">Mac</a>, <a href="https://slack.com/ssb/download-win">Windows</a>)
- Sublime Text (<a href="https://download.sublimetext.com/Sublime%20Text%20Build%203114.dmg">Mac</a>, <a href="https://download.sublimetext.com/Sublime%20Text%20Build%203114%20x64%20Setup.exe">Windows</a>)
- <a href="https://desktop.github.com/">Github Desktop App</a>
- Tabula (<a href="https://github.com/tabulapdf/tabula/releases/download/v1.0.1/tabula-mac-1.0.1.zip">Mac</a>, <a href="https://github.com/tabulapdf/tabula/releases/download/v1.0.1/tabula-win-1.0.1.zip">Windows</a>)
- Open Refine (<a href="https://github.com/OpenRefine/OpenRefine/releases/download/2.5/google-refine-2.5-r2407.dmg">Mac</a>, <a href="https://github.com/OpenRefine/OpenRefine/releases/download/2.5/google-refine-2.5-r2407.zip">Windows</a>)
	- If you're on a Mac, and you get the error that Google/Open Refine is damaged, [follow these instructions](open-refine-troubleshooting.md).

**Macs**
- Open your <a href="https://en.wikipedia.org/wiki/Terminal_(OS_X)">Terminal app</a> (comes with all Macs) and paste these exact commands into the window, one at a time, and press enter:
- `xcode-select --install`
- `python -V`
  - Your Terminal should say something like "Python 2.7.13". Your last two digits might be different, that's okay. If you get something that Python 3, which looks like: "Python 3.X.XX" let Sisi know.
- `curl https://bootstrap.pypa.io/get-pip.py | sudo python`
  - This will ask you to put in your computer password. Go ahead, and quick warning: the cursor won't move, but trust that your computer is reading what you're typing in.
- `pip install --user BeautifulSoup`
- `pip install --user Requests`

**Windows**
- Download [Cygwin](https://cygwin.com/install.html)
	- Here's a [screenshot-by-screenshot walkthrough](http://www.mcclean-cooper.com/valentino/cygwin_install/) of what installing it should be like. 
	- **PLEASE NOTE:**
		- On step 9, installing packages, you only need to select `python`and `git` as packages to install. If there are multiple versions of `python` options, pick `python2`. 
		- Only go through steps 1-10. **Do not** continue to the "Setup Notes" section of the walkthrough.

<hr/>

## Day 1
### Monday, July 22

### Intro to Data Journalism
<a href="https://projects.propublica.org/graphics/images/data-institute/presentations/2019/intro-to-data.pdf"><img width="300" src="https://projects.propublica.org/graphics/images/data-institute/presentations/2019/intro-to-data.jpg"></a>

<a href="https://projects.propublica.org/graphics/images/data-institute/presentations/2019/intro-to-spreadsheets.pdf"><img width="300" src="https://projects.propublica.org/graphics/images/data-institute/presentations/2019/intro-to-spreadsheets.jpg"></a>

**Exercises**
- Organizing information in rows & columns using [biographical information](http://bioguide.congress.gov/biosearch/biosearch.asp)
- Learning how to sort with [Trump expenditures](https://docs.google.com/spreadsheets/d/1od86DSRi5kJPJfLpDRcSbPj2nJiRk4yJUIrfunjlK4Q/edit#gid=0)

<a href="https://projects.propublica.org/graphics/images/data-institute/presentations/2019/finding-data.pdf"><img width="300" src="https://projects.propublica.org/graphics/images/data-institute/presentations/2019/finding-data.jpg"></a>

<a href="https://projects.propublica.org/graphics/images/data-institute/presentations/2019/loading-data.pdf"><img width="300" src="https://projects.propublica.org/graphics/images/data-institute/presentations/2019/loading-data.jpg"></a>

**In-Class Demos**
- Using Socrata to look at [3-1-1 calls from NYC](https://nycopendata.socrata.com/Social-Services/311-Service-Requests-from-2010-to-Present/erm2-nwe9)
- [Tabula](https://tabula.technology/)
- Types of data (numeric, text, date)
- Quirks of Excel (reformatting dates, dropping leading zeros)
- Text files and types (csv, tab, fixed width, pipe)
- Text delimiter (probably quotes, but maybe not)
- Open your text file in a reader and examine it

<a href="https://projects.propublica.org/graphics/images/data-institute/presentations/best-practices.pdf"><img width="300" src="https://projects.propublica.org/graphics/images/data-institute/presentations/best-practices.jpg"></a>

**In-Class Demos**
- Create a text document
- Save a clean copy of your data
- Keep track of your work
- Describe your steps
- Copy/paste functions
- Screen grabs of dialogue boxes

### Advanced Spreadsheets: Pivot Tables

### Advanced Spreadsheets: String Functions
<a href="https://projects.propublica.org/graphics/images/data-institute/presentations/string-functions.pdf"><img width="300" src="https://projects.propublica.org/graphics/images/data-institute/presentations/string-functions.jpg"></a>

**Exercises**
- [Practice Data](https://drive.google.com/file/d/0Bw5Mt7QIQlsgc2tLdFlpQ2QwTXM/view)
- Reformat
- Split
- Transpose

### Homework
- None! Enjoy the city!

## Day 2
### Tuesday, July 23

<a href="https://projects.propublica.org/graphics/images/data-institute/presentations/evaluating-data.pdf"><img width="300" src="https://projects.propublica.org/graphics/images/data-institute/presentations/evaluating-data.jpg"></a>

**Exercises**
- [Fairfax Arrests](https://www.strongspace.com/shared/u6n69debcw)

<a href="https://projects.propublica.org/graphics/images/data-institute/presentations/2017/data-integrity.pdf"><img width="300" src="https://projects.propublica.org/graphics/images/data-institute/presentations/2017/data-integrity.jpg"></a>

<a href="https://projects.propublica.org/graphics/images/data-institute/presentations/open-refine.pdf"><img width="300" src="https://projects.propublica.org/graphics/images/data-institute/presentations/open-refine.jpg"></a>

<a href="https://projects.propublica.org/graphics/images/data-institute/presentations/one-var.pdf"><img width="300" src="https://projects.propublica.org/graphics/images/data-institute/presentations/one-var.jpg"></a>

### Advanced Spreadsheets: Combining Two Sheets with VLOOKUP

### Homework
- None! Enjoy the city!

## Day 3
### Wednesday, July 24

### Mapping

- [John Snow's map](https://www1.udel.edu/johnmack/frec682/cholera/)
- [Census Geocoder](https://geocoding.geo.census.gov/geocoder/locations/addressbatch?form)

**Exercise***
- [Bill de Blasio donors](https://docs.google.com/spreadsheets/d/17NlwDllhkKCDLa1cnKJDelQhcAjt4yRS2YJeQnGG-ao/edit#gid=0)
- [Datawrapper](https://www.datawrapper.de/)

### Analyzing Data, continued
- [Histograms revisited](https://docs.google.com/presentation/d/1tUJgdvNVnAiX9GOa2t6_ZHL4iKB01jc6eOWEuP77ZiY/edit?usp=sharing)
- [Data Analysis Grab-Bag (slides)](https://docs.google.com/presentation/d/1WD0NiqrmYQCMpkN7cCyIAbntjXEVqzmrjP7HQYOnVzY/edit?usp=sharing)
	- percent change
	- percapita
	- choosing your denominator wisely
	- correlation
- [Two Variables (slides)](https://drive.google.com/file/d/0Bw5Mt7QIQlsgMDl4UE9CZ1F0c1E/view?usp=sharing)
	- scatterplots
	- fitting a line
- [Statistical Tests with M&Ms](https://drive.google.com/open?id=0Bw5Mt7QIQlsgaDgyODFlUjNTQ0E)
- Resources
	- [Numbers in the Newsroom: Using Math and Statistics in News](https://store.ire.org/products/numbers-in-the-newsroom-using-math-and-statistics-in-news-second-edition-e-version) by Sarah Cohen
	- [Precision Journalism: A Reporter's Introduction to Social Science Methods](https://www.amazon.com/Precision-Journalism-Reporters-Introduction-Science/dp/0742510883) by Philip Meyer
	- [Google Sheets Tutorials](https://training.npr.org/visual/what-to-do-with-a-big-pile-of-data/)

### Homework
- None! Enjoy the city!

<!--

## Day 4
### Thursday, July 25

### Intro to Code
<a href="https://projects.propublica.org/graphics/images/data-institute/presentations/2017/intro-to-code.pdf"><img width="500" src="https://projects.propublica.org/graphics/images/data-institute/presentations/intro-to-code.jpg"></a>

**In-Class Demos**
- What coding languages have you heard of?
- Using the web inspector

### How Websites Work
<a href="https://projects.propublica.org/graphics/images/data-institute/presentations/2017/how-websites-work.pdf"><img width="500" src="https://projects.propublica.org/graphics/images/data-institute/presentations/2017/how-websites-work.jpg"></a>

**In-Class Demos**
- How the Internet passes websites around
- What HTML, CSS and Javascript contribute to a webpage

**Exercises**
- Drawing a Website

### HTML
<a href="https://projects.propublica.org/graphics/images/data-institute/presentations/2017/html.pdf"><img width="500" src="https://projects.propublica.org/graphics/images/data-institute/presentations/html.jpg"></a>

**In-Class Demos**
- How to create your first HTML file
- Shortcut to the basic HTML template
- How to use:
  - `<h1>`
  - `<h2>`
  - `<h3>`
  - `<p>`
  - `<img>`
  - `<a>`
  - `<ul>`


**Exercises**
<ul>
  <li>Copy and paste <a href="https://codepen.io/sisiwei/pen/KzLezJ?editors=1000">this code</a> and follow the instructions inside to format the page.</li>
  <li>Can you fix this <a href="https://codepen.io/sisiwei/pen/PNvaeB?editors=1000">broken code</a>? </li>
</ul>

### Basic CSS
<a href="https://projects.propublica.org/graphics/images/data-institute/presentations/2017/css.pdf"><img width="500" src="https://projects.propublica.org/graphics/images/data-institute/presentations/2017/css.jpg"></a>

**In-Class Demos**
<ul>
  <li>How to create your first CSS file</li>
  <li>Shortcut to linking to your CSS file</li>
  <li>How CSS styles work</li>
</ul>

**Exercises**
<ul>
  <li>Using your practice HTML file from before, add CSS styles to it such you change the:
    <ul>
      <li>color</li>
      <li>font-family</li>
      <li>font-size</li>
    </ul>
  </li>
  <li>On your own, look up how to do the following in CSS, and add it to your HTML file as well:
    <ul>
      <li>underline text</li>
      <li>bold text</li>
      <li>italicize text</li>
    </ul>
  </li>
  <li>Going back to the Supreme Court article you formatted earlier, do the following using CSS:
    <ul>
      <li>Make the main headline dark red.</li>
      <li>Use the font family "Georgia" for the main headline and the subheadline.</li>
      <li>Center the text of the main headline and the subheadline.</li>
      <li>Give the paragraphs a line height of 19 pixels.</li>
      <li>Remove the underline from the links.</li>
      <li>Make the "Related articles" label all uppercase.</li>
      <li>Bonus: Make an underline appear when you hover over a link.</li>
    </ul>
  </li>
</ul>

### CSS Classes

**In-Class Demos**
<ul>
  <li>How to write your own CSS Class</li>
  <li>How CSS deals with conflict</li>
</ul>

### Homework

<ul>
  <li>Save <a href="https://codepen.io/sisiwei/pen/bpXwMB?editors=1000">this HTML</a> onto your computer. Link to a new CSS file that you create. Write CSS to make the end result look like <a href="http://projects.propublica.org/graphics/images/data-institute/presentations/mars.jpg">this image</a>. You may only write CSS. You cannot edit the HTML file.</li>
  <li>Using HTML and CSS, lay out a one-page web portfolio for yourself. Don't worry too much about the final design, though you are free to get started designing. Just make sure to get all of your information on the page and formatted using HTML.</li>
</ul>

## Day 5
### Friday, July 26

### Intro to Design
<p>
<a href="https://lenagroeger.com/design_workshop" target="_blank">
  <img src="https://propublica.s3.amazonaws.com/projects/datainstitute/lena/imgs/design_intro.jpg">
</a>
</p>


**Lecture**
<ul>
  <li>What's Design Anyways?</li>
  <li>Design Principles: The Only 4 Rules You Gotta Know</li>
</ul>

**Exercises**
<ul>
  <li>Align This!</li>
  <li>Resume Redesign</li>
</ul>


### Type, Layout & Color
<p>
<a href="https://propublica.s3.amazonaws.com/projects/datainstitute/lena/lectures/TypeLayoutColor.pdf" target="_blank"><img width="500" src="https://propublica.s3.amazonaws.com/projects/datainstitute/lena/imgs/type.jpg"></a>
</p>

**Lecture**
<ul>
  <li>Letter: The Many Faces of Type</li>
  <li>Text: How to Deal with Words</li>
  <li>The Grid: Putting the Pieces Together</li>
  <li>Colors &amp; How to Pick 'Em </li>
</ul>



**Exercises**
<ul>
  <li>Name that Font!</li>
  <li>Type Crimes</li>
</ul>


### Let's make a webpage!

<p>
<a target="_blank" href="http://lenagroeger.com/makeawebsite/"><img width="500" src="https://propublica.s3.amazonaws.com/projects/datainstitute/lena/imgs/online_portfolio.jpg"></a>
</p>

**Exercises**       
<ul>
  <li><a target="_blank" href="http://lenagroeger.com/makeawebsite/">Making a website</a></li>
  <li>Getting your portfolio on the internet!</li>
  <li>Using the GitHub Desktop app</li>
</ul>



### Homework
<ul>
  <li>Using the principles we discussed today, redesign your résumé. Email the before and after version to <a href="mailto:lena.groeger@propublica.org">lena.groeger@propublica.org</a>.</li>
  <li>Using everything you've learned about design, type & layout, keep working on your portfolio HTML page. Then, since you've learned how to make a working webpage on the internet, upload your page to Github.</li>
</ul>



<br></br>
<h2>📚 Weekend! 🎉</h2>



## Day 6
### Monday, July 29

### Javascript and JQuery

**Review**  
- Making a Website with Cards ♠️
- Reminder to send Lena your resumes!
- Going over homework from last Thursday

**In-Class Demos**  
- How to setup Javascript
- How to add jQuery, set it up, and use it ([A good place to review what we're learning](https://www.w3schools.com/jquery/jquery_intro.asp))
- Ida Demo: [Starting with this HTML and CSS](https://codepen.io/sisiwei/pen/ZWdXGw), let's build the JS together.

**Exercises**
- Save [this code](https://codepen.io/sisiwei/pen/MmZvgy) onto your computer as separate HTML and CSS files. Create a new JS - file and link to it in your HTML.
- Let's talk through logically, what needs to happen together.
- Can you figure out how to build a before and after graphic using Javascript?

**Homework**
- Using your own photos, make your own before and after interactive. Then, publish your interactive on Github and add it to your portfolio.
- Create an account for [Datawrapper](https://app.datawrapper.de/signin) before tomorrow.

## Day 7
### Tuesday, July 30

### Visualizing Data
<p>
  <a target="_blank" href="https://lenagroeger.com/visualizing-data/"><img width="500" src="https://propublica.s3.amazonaws.com/projects/datainstitute/lena/imgs/visualizing_data.jpg"></a>
</p>

**Lecture**
<ul>
  <li>Lines</li>
  <li>Bars</li>
  <li>Scatterplots, Treemaps &amp; More!</li>
</ul>


### Let's Make Some Charts & Maps!

<p>
  <a href="https://www.datawrapper.de/"><img width="500" src="https://propublica.s3.amazonaws.com/projects/datainstitute/lena/imgs/datawrapper.jpg">
  </a>
</p>

**In-Class Demos**  
<ul>
  <li>From data to charts in Google Sheets &amp; Data Wrapper</li>
</ul>


**Exercises**
<ul>
  <li><a href="https://lenagroeger.com/datawrapper/">Making Maps & Charts in Datawrapper!</a></li>
</ul>


## Day 8
### Wednesday, July 31

### Web Scraping + Fundamentals of Programming
**In-Class Demos**
<ul>
  <li>Introduction to Web Scraping</li>
  <li>Thinking through how to scrape <a href="https://report.boonecountymo.org/mrcjava/servlet/SH01_MP.I00290s">this website</a></li>
  <li>Download and unzip <a href="https://propublica.s3.amazonaws.com/projects/datainstitute/jailscrape.zip">this folder</a> into your "Code" folder on your computer</li>
  <li>Fundamentals of Programming</li>
  <li>Want to review later? Everything we're covering is <a href="https://first-web-scraper.readthedocs.io/en/latest/#act-2-python">laid out here</a>.</li>
</ul>

**Exercises**

We'll do the first two together, and you'll do the rest on your own.

1. Write a function, named `copycat`, that simply prints out whatever input it's given.
2. Write a function, named `addition`, that when given any three numbers, will print out the total sum of all three numbers.
3. Write a function, named `conversion`, that when given the Fahrenheit temperature, will print out what it is in Celsius. The formula you can use is: `C = (F – 32) * 5/9`
4. Write a function, named `find_the_max`, that given any three numbers, will print out the bigger number. Python has the native ability to do this, using the function `max()`. Do not use it. Instead write this from scratch.
5. <strong>For an extra challenge:</strong> Given the following data, write a function, named `total_students`, that calculates how many total students are enrolled in Hogwarts. <br/>
`pupils_by_year = [["first years", 40], ["second years", 40], ["third years", 38], ["fourth years", 35], ["fifth years", 30], ["sixth years", 29], ["seventh years", 23]]`


**Homework**
<ul>
  <li>Keep working on your portfolios and presentations.</li>
  <li>See if you can write yourself any other functions. It'll help you gear up for tomorrow.</li>
</ul>

## Day 9
### Thursday, August 1

### Web Scraping, Continued

**In-Class Demos**
- Even more web scraping!

**Homework**
<ul>
  <li>Prepare your presentation for tomorrow! Send a URL of the project you want to show to <a href="mailto:data.institute@propublica.org">data.institute@propublica.org</a> by tomorrow at 9:30am. Here are some questions to think about: </li>
  <li><b>General</b>: What did you learn? What can you do now that you could not do 2 weeks ago? What were the biggest challenges/setbacks/frustrations you faced? The biggest surprises/succeses/most awesome things you accomplished? </li>
  <li><b>Project specific</b>: Tell us what you’re presenting: your portfolio, a dataset you analyzed, a data visualization you created. What are you proud of? What are the next steps you want to take? What are your ultimate goals for the project?</li>
</ul>

## Day 10
### Friday, August 2
 -->
