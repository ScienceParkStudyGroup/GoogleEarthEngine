---
title: "GEE Access and JavaScript Tips"
teaching: 0
exercises: 0
questions:
- How do I get an account?
- What are some JavaScript basics?
objectives:
- Gain access to Google Earth Engine
- Have a JavaScript resource
keypoints:
- "Anyone can sign up for Google Earth Engine, just apply to be a trusted tester."
- "The Code Editor is a user friendly access point for Earth Engine that uses the JavaScript IDE."
- " JavaScript is a programming language that is also widely used in web development."
---
# Prerequisites

Use the steps below to register for a Google Earth Engine account and to join our shared repository.

### 1. Registering for a Google Earth Engine account

  - Go the the [GEE sign up page](https://signup.earthengine.google.com/#!/) and enter > the email you want to use for your GEE account. A gmail is best if you have one.
  - Enter your email, your affiliation and country/region. Where it asks what you want to accomplish, mention: Amsterdam Science Park Study Group workshop.
  - Review the terms, verify your non-robot identify and click 'Submit'.
  - Check your email, including your spam folder, for a link from the Google Developer's Team. The confirmation email will have directions on how to access the Code Editor.

Not sure if you have access? Use [this link](https://code.earthengine.google.com/) to check. If you didn't get access you will get an authorization error that says your account isn't registered. If you do have access, the link will open up the Javascript IDE. This link is your permanent portal to GEE access.

### 2. Joining our shared GEE code repository

Google Earth Engine allows you to have shared group folders/repositories for scripts. Use the following link to access the workshop material. The course material is an updated version of the material developed for the geohackweek 2018. Open the shared repository by clicking this link:

  -  <a href="https://code.earthengine.google.com/?accept_repo=users/johannesdegroeve/GEE_SPSG_2021
" target="_blank">https://code.earthengine.google.com/?accept_repo=users/johannesdegroeve/GEE_SPSG_2021</a>
  - In the code editor, go to the **Scripts tab** in the top left panel, scroll down and expand the "Reader" section. A directory called *users/johannesdegroeve/GEE_SPSG_2021* should appear with read-only versions of the full scripts from each episode.
  - Please make another repository in the "Owner" section with a name of choice and make a first script "02-CodeEditor". You can use that repository as your working environment for the excercises. 

### 3. Javascript Tips

JavaScript, not to be confused with Java, is a programming language widely used in web development alongside HTML and CSS. In this course we access Google Earth Engine by entering JavaScript commands into an online integrated development environment (IDE) called the Code Editor. It is not necessary to formally learn JavaScript to work with Google Earth Engine. 

There are many online tutorials for learning JavaScript, but the <a href="https://developers.google.com/earth-engine/tutorials/tutorial_js_01" target="_blank">Introduction to JavaScript for Earth Engine</a> guide is most applicable if you want to learn more after this course. Below we provide examples and resources for getting started.  

#### Basic JavaScript for GEE
Here are a few basics useful for GEE, reproduced from the <a href="https://docs.google.com/document/d/1ZxRKMie8dfTvBmUNOO0TFMkd7ELGWf3WjX0JvESZdOE/edit" target="_blank">Earth Engine 101 Beginner's Curriculum</a>.



{% highlight javascript %}
// Line comments start with two forward slashes. Like this line.

/* Multi-line comments start with a forward slash and a star,
and end with a star and a forward slash. */
{% endhighlight %}

Variables are used to store objects and are defined using the keyword **var**.
{% highlight javascript %}
var theAnswer = 42;

// string objects start and end with a single quote
var myVariable = 'I am a string';

// string objects can also use double quotes, but don't mix and match
var myOtherVariable = "I am also a string";
{% endhighlight %}

Statements should end in a semi-colon, or the editor complains.
{% highlight javascript %}
var test = 'I feel incomplete...'
var test2 = 'I feel complete!';
{% endhighlight %}

Passing function parameters and using lists
{% highlight javascript %}
// Parentheses are used to pass parameters to functions
print('This string will print in the Console tab.');

/* Square brackets are used for items in a list.
The zero index refers to the first item in a list*/
var myList = ['eggplant','apple','wheat'];
print(myList[0]); // would print 'eggplant'
{% endhighlight %}

Using dictionaries
{% highlight javascript %}
// Curly brackets (or braces) can be used to define dictionaries (key:value pairs).
var myDict = {'food':'bread', 'color':'red', 'number':42};

// Square brackets can be used to access dictionary items by key.
print(myDict['color']);

//Or you can use the dot notation to get the same result.
print(myDict.color);
{% endhighlight %}

Functions can be defined as a way to reuse code and make it easier to read.
{% highlight javascript %}
var myHelloFunction = function(string) {
  return 'Hello ' + string + '!';
};
print(myHelloFunction('world'));
{% endhighlight %}


#### Other JavaScript Resources
JavaScript uses camelCase. JavaScript (according to W3 academy) is easy to learn. Like other programming languages, you can use style guides to learn how to write standard, reproducible (marketable!) code.

For in-depth industry guidance, Google publishes their own definitive <a href="http://google.github.io/styleguide/jsguide.html" target="_blank">JavaScript style guide</a>.

Google Earth Engine provides extensive guides and <a href="https://developers.google.com/earth-engine/tutorials" target="_blank">educational resources</a> in case you want to learn more after this course.


<br>
<img src="../fig/00_spaceland.png" border = "10">
<br><br>
