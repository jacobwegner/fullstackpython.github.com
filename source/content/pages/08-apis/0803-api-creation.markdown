title: API Creation
category: page
slug: api-creation
sort-order: 0803
choice1url: /application-programming-interfaces.html
choice1icon: fa-exchange
choice1text: What are application programming interfaces?
choice2url: /api-integration.html
choice2icon: fa-link
choice2text: How do I integrate external APIs into my application?
choice3url: /web-application-security.html
choice3icon: fa-lock fa-inverse
choice3text: How can I learn about web application security?
choice4url: /static-content.html
choice4icon: fa-spinner fa-inverse
choice4text: Where should I host static content such as JavaScript files?


# API Creation
Creating and exposing APIs allows your web application to interact with other
applications through machine-to-machine communication.


## API creation frameworks
* [Django REST framework](http://www.django-rest-framework.org/) and
  [Tastypie](https://django-tastypie.readthedocs.org/en/latest/) are 
  the two most widely used API frameworks to use with Django. The edge
  currently goes to Django REST framework based on rough community sentiment.

* [Flask-RESTful](http://flask-restful.readthedocs.org/en/latest/) and
  [Flask API](http://flask.pocoo.org/docs/api/) are popular libraries for 
  exposing APIs from Flask web applications.

* [Sandman](http://www.github.com/jeffknupp/sandman) is a widely used tool to
  automatically generate a RESTful API service from a legacy database without
  writing a line of code (though it's easily extensible through code).

* [Cornice](https://cornice.readthedocs.org/en/latest/) is a REST framework
  for Pyramid.

* [Restless](https://github.com/toastdriven/restless) is a lightweight API
  framework that aims to be framework agnostic. The general concept is that
  you can use the same API code for Django, Flask, Bottle, Pyramid or any
  other WSGI framework with minimal porting effort.

* [Eve](http://python-eve.org/) is a Python REST framework built with Flask,
  MongoDB and Redis. The framework's primary author 
  [Nicola Iarocci](https://twitter.com/nicolaiarocci) gave a great talk at 
  [EuroPython 2014](https://www.youtube.com/watch?v=9sUsLvG72_o) that 
  introduced the main features of the framework.


## API testing projects
Building, running and maintaining APIs requires as much effort as building,
running and maintaining a web application. API testing frameworks are the 
equivalent of browser testing in the web application world.

* [zato-apitest](https://github.com/zatosource/zato-apitest) invokes HTTP 
  APIs and provides hooks for running through other testing frameworks.



## Hosted API testing services
* [Runscope](https://www.runscope.com/) is an API testing SaaS application
  that can test both your own APIs and external APIs that your application
  relies upon.

* [API Science](https://www.apiscience.com/) is focused on deep API testing,
  including multi-step API calls and monitoring of external APIs.

* [SmartBear](http://smartbear.com/api-testing/) has several API monitoring
  and testing tools for APIs.


## API creation resources
* [NARWHL](http://www.narwhl.com/) is a practical API design site for 
  developers confused about what is appropriate for RESTful APIs.

* This [API Design Guide](https://github.com/interagent/http-api-design) 
  is based on Heroku's best practices for the platform's API.

* [18F](https://18f.gsa.gov/)'s 
  [API standards](https://github.com/18f/api-standards) explains the details
  behind their design decisions on creating modern RESTful APIs.

* [Choosing an API framework for Django](http://pydanny.com/choosing-an-api-framework-for-django.html)
  by [PyDanny](https://twitter.com/pydanny) contains questions and insight
  into what makes a good API framework and which one you should currently
  choose for Django.

* [RESTful web services with Python](http://www.slideshare.net/Solution4Future/python-restful-webservices-with-python-flask-and-django-solutions)
  is an interesting overview of the Python API frameworks space.

* [10 Reasons Why Developers Hate Your API (And what to do about it)](http://www.slideshare.net/jmusser/ten-reasons-developershateyourapi)
  goes through the top difficulties and annoyances developers face when
  working with APIs and how you can avoid your API falling into the same
  traps.

* "[Design a beautiful REST API](https://medium.com/@zwacky/design-a-beautiful-rest-api-901c73489458)"
  reviews common design decisions regarding endpoints, versioning, errors and
  pagination. There is also a 
  [source material YouTube video](https://www.youtube.com/watch?v=5WXYw4J4QOU)
  where this blog post derives its recommendations from.

* "[Self-descriptive, isn't. Don't assume anything.](http://www.bizcoder.com/self-descriptive-isn-t-don-t-assume-anything)"
  is an appeal that metadata makes a difference in whether APIs are descriptive
  or not.


## API creation learning checklist
<i class="fa fa-check-square-o"></i>
Pick an API framework appropriate for your web framework. For Django I 
recommend Django REST framework and for Flask I recommend Flask-RESTful.

<i class="fa fa-check-square-o"></i>
Begin by building out a simple use case for the API. Generally the use case
will either involve data that users want in a machine-readable format or a
backend for alternative clients such as an iOS or Android mobile app.

<i class="fa fa-check-square-o"></i>
Add an authentication mechanism through OAuth or a token scheme.

<i class="fa fa-check-square-o"></i>
Add rate limiting to the API if data usage volume could be a performance issue.
Also add basic metrics so you can determine how often the API is being 
accessed and whether it is performing properly.

<i class="fa fa-check-square-o"></i>
Provide ample documentation and a walkthrough for how the API can be accessed
and used.

<i class="fa fa-check-square-o"></i>
Figure out other use cases and expand based on what you learned with the 
initial API use case.


### What's next after building an API for your web app?
