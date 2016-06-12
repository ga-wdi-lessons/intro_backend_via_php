# Intro to the Back-end via PHP

## Learning Objectives
- HTTP methods
- GET, POST
- Headers vs body
- Cookies
- Index
- Templating engine
- Difference between front-end and back-end
- ID which languages are used on which end
- Nameserver and DNS

## Request/Response Cycle

A **server** is a computer that receives **requests** for data and **responds** to them. It "serves" data.

The job of your browser is to "interpret" the data.

### Example flow

1. You type "www.generalassemb.ly" into your browser
- Your browser sends a **request** to GA's server for that URL
- GA's server looks up a rule written by one of GA's back-end developers that says, "When someone requests www.generalassemb.ly, send them this file"
- GA's server finds the appropriate file
- GA's server **responds** with the file
- Your browser receives the file
- Your browser notices the images, stylesheets, and javascripts linked in the HTML and makes a request for each of them
- Your browser executes all the CSS and JS

### What's in a request?

A request is much more than simply, "This is the URL I want."

Go to this page:

http://putsomethinghere.com/php/global.php

> This is a web domain I own but am not using at the moment.

Everything beginning with `HTTP` is a header that was sent by the request you just made to my server.

### You do: Set a header

Go to [Hurl.it](https://www.hurl.it/). In the "Destination", put:

```
http://putsomethinghere.com/php/global.php
```

- What do you see?

Now "Add Header". It can be anything you want. I tried a `name` of "Turtle" and a `value` of "Soup".

- Look for "Turtle" in the response. Where is it?



### GET and POST (and the rest)

## Dynamic Pages and Templating

### Analogy: The theater

An actor takes a bunch of text and turns it into something *more* than text: a play.

A web browser takes a bunch of text and turns it into something *more* than text: a webpage.

A server is what provides the text in the first place.

### Restricting data

#### Shakespeare

Consider: Shakespeare is commissioned at the same time to write a play for Spain and a play for England. He's efficient so he sends the same play to both. The only change he makes between the two copies is the British version mocks the Spanish monarchy, and the Spanish version mocks the British monarchy.

#### Contact info

My website, RobertAKARobin.com, is my resume, and can be printed out like one.

Usually you include your street address and phone number on your resume. However, I don't want my contact information to be visible to everyone.

I could use Javascript or CSS to hide this information, but anyone would be able to look at my source code to see it.

So, on the back-end of my site I have a rule that says, "If I'm accessing this site from my computer, show my number and address. Otherwise, hide them."

## References
- Famous interview question: [What happens when you type google.com into your browser's address box and press enter?](https://github.com/alex/what-happens-when)
