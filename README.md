# Developing a Simple Webserver
## AIM:
To develop a simple webserver to serve html pages.

## DESIGN STEPS:
### Step 1: 
HTML content creation
### Step 2:
Design of webserver workflow
### Step 3:
Implementation using Python code
### Step 4:
Serving the HTML pages.
### Step 5:
Testing the webserver

## PROGRAM:
```
from http.server import HTTPServer, BaseHTTPRequestHandler
content = """
<!DOCTYPE html>
<html>
<head>
<title>Programmers World</title>
</head>
<body>
<h1><marquee>Welcome to The Programmers World</marquee></h1>
<body text = "white">
<style>
body {
  background-image: url('https://cdn.wallpapersafari.com/65/57/me7zqw.jpg');
  background-repeat: no-repeat;
  background-attachment: fixed;
  background-size: cover;
}
</style>
<body style = "font-family:Courier New;" >
<h2><p align = "center">Here You Will Learn About The Top 5 Programming Languages</br> In The World</p></h2>
<h2>Currently The Top 5 Languages Are :</h2>
<h2><b>1. JavaScript</br>2. Python</br>3. C/C++</br>4. Java</br>5. R Language</b><h2>
<h2><p align = "center">JAVASCRIPT</p><h2><img src="https://cdn.icon-icons.com/icons2/2108/PNG/512/javascript_icon_130900.png" alt="Java Script" width="200px" height="200px" style="float:right">
</br>
JavaScript is a lightweight, cross-platform, and interpreted scripting language. It is well-known for the development of web pages, many non-browser environments also use it. JavaScript can be used for Client-side developments as well as Server-side developments.</br> 
</br>
JavaScript contains a standard library of objects, like Array, Date, and Math, and a core set of language elements like operators, control structures, and statements. 
JavaScript was initially created to “make web pages alive”.</br>
</br>
The programs in this language are called scripts. They can be written right in a web page’s HTML and run automatically as the page loads.</br>
Scripts are provided and executed as plain text. They don’t need special preparation or compilation to run.</br>
</br>
In this aspect, JavaScript is very different from another language called Java.</br>
</br>
To learn Javascript Coding and more information regarding it ,click on the link below.</br> 
<a href="https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/JavaScript_basics"> Reference Link</a>
<h2><p align = "center">PYTHON</p></h><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/c/c3/Python-logo-notext.svg/1200px-Python-logo-notext.svg.png" alt="pYTHON" width="200px" height="200px" style="float:right">
</br>
Python is a widely used general-purpose, high level programming language. It was created by Guido van Rossum in 1991 and further developed by the Python Software Foundation. It was designed with an emphasis on code readability, and its syntax allows programmers to express their concepts in fewer lines of code.</br>
</br>
Python is a programming language that lets you work quickly and integrate systems more efficiently.</br>
</br>
It is also called general-purpose programming language as it is used in almost every domain we can think of as mentioned below:</br>
</br>
Web Development</br>
Software Development</br>
Game Development</br>
AI & ML</br>
Data Analytics</br>
</br>
To learn Python Coding and more information regarding it ,click on the link below.</br> 
<a href="https://www.python.org/about/gettingstarted/"> Reference Link</a>
<h2><p align = "center">C/C++</p></h><img src="https://docs.microsoft.com/cs-cz/windows/images/c-logo.png" alt="C/C++" width="200px" height="200px" style="float:right">
</br>
C++ is a general-purpose programming language that was developed as an enhancement of the C language to include object-oriented paradigm. It is an imperative and a compiled language.</br>
</br>
C++ is a middle-level language rendering it the advantage of programming low-level (drivers, kernels) and even higher-level applications (games, GUI, desktop apps etc.). The basic syntax and code structure of both C and C++ are the same. </br>
</br>
Simple: It is a simple language in the sense that programs can be broken down into logical units and parts, has a rich library support and a variety of data-types.</br>
</br>
Machine Independent but Platform Dependent: A C++ executable is not platform-independent (compiled programs on Linux won’t run on Windows), however they are machine independent.</br>
</br>
<h2><p align = "center">JAVA</p></h><img src="https://1000logos.net/wp-content/uploads/2020/09/Java-Logo.png" alt="Java" width="300px" height="200px" style="float:right">
</br>
JAVA was developed by James Gosling at Sun Microsystems Inc in the year 1991, later acquired by Oracle Corporation. It is a simple programming language. Java makes writing, compiling, and debugging programming easy. It helps to create reusable code and modular programs.</br>
</br>
Java is a class-based, object-oriented programming language and is designed to have as few implementation dependencies as possible. A general-purpose programming language made for developers to write once run anywhere that is compiled Java code can run on all platforms that support Java. Java applications are compiled to byte code that can run on any Java Virtual Machine. The syntax of Java is similar to c/c++.</br>
</br>
It is used for:</br>
</br>
Mobile applications (specially Android apps)</br>
Desktop applications</br>
Web applications</br>
Web servers and application servers</br>
Game Development</br>
Database connection</br>
</br>
To learn C & C++ Coding and more information regarding it ,click on the link below.</br> 
<a href="https://www.programiz.com/c-programming"> Reference Link For C</a></br>
<a href="https://www.programiz.com/cpp-programming"> Reference Link For C++</a>
<h2><p align = "center">R LANGUAGE</p></h><img src="https://www.logolynx.com/images/logolynx/c3/c3b7ed5d007115f23b737150df873247.png" alt="R Language" width="200px" height="200px" style="float:right">
</br>
R is an open-source programming language that is widely used as a statistical software and data analysis tool. R generally comes with the Command-line interface. R is available across widely used platforms like Windows, Linux, and macOS. Also, the R programming language is the latest cutting-edge tool.</br>
</br>
It was designed by Ross Ihaka and Robert Gentleman at the University of Auckland, New Zealand, and is currently developed by the R Development Core Team. R programming language is an implementation of the S programming language. It also combines with lexical scoping semantics inspired by Scheme. Moreover, the project conceives in 1992, with an initial version released in 1995 and a stable beta version in 2000.</br>
</br>
Data analysis with R is done in a series of steps; programming, transforming, discovering, modeling and communicate the results.</br>
</br>
Program: R is a clear and accessible programming tool</br>
Transform: R is made up of a collection of libraries designed specifically for data science</br>
Discover: Investigate the data, refine your hypothesis and analyze them</br>
Model: R provides a wide array of tools to capture the right model for your data
Communicate: Integrate codes, graphs, and outputs to a report with R Markdown or build Shiny apps to share with the world</br>
</br>
To R Language and more information regarding it ,click on the link below.</br> 
<a href="https://www.tutorialspoint.com/r/index.htm"> Reference Link</a>
<h2><marquee>Thank For Visiting Our Page</marquee</h2>
<h2><marquee>Hope That The Information Was Useful</marquee></h2>

</body>
</html>


"""
class myhandler(BaseHTTPRequestHandler):
    def do_GET(self):
        print("request received")
        self.send_response(200)
        self.send_header('content-type', 'text/html; charset=utf-8')
        self.end_headers()
        self.wfile.write(content.encode())
server_address = ('',8080)
httpd = HTTPServer(server_address,myhandler)
print("my webserver is running...")
httpd.serve_forever()

```

## OUTPUT:


## RESULT:
