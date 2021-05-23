# m3
Milestone Project 3
Python and Data Centric Develpment.

THE PAPER FOLK

In this milestone project I am to create a book recommendation website that allows the end user to store their data or "tastes",
after filling in a questionnaire on their profile. The website owner would recive a finders fee after the end user makes a purchase
with the merchant provided by the book recommendation website.  

This will highlight my ability to create a functioning Data centric website, work with flask as a basic framework 

The addition of a social media or blog like feature would allow for more user interaction

I am to create a website that allows users to interact with a book database (MongoDB)

Using Git Bash as a vertual enviroment, I will use create a basic flask website framework.

i created a directory using Git bash, I then installed flask into the directory. 

Start Virtual enviroment 
1.Open Git bash 
2.use "cd /c/my_flask/" to root to the apps directory
3.start virtual enviroment "source virtual/scripts/activate", "deactivate" (to turn off)
4.type "flask run" to launch enviroment on http://127.0.0.1:5000/ (local host) 
5."ctrl, and c" to close local host

Lazy development or lazy loading: (this allows for instant updating of files for website)
1.export FLASK_APP=app.py (app.py will update live)
2.export FLASK_ENV=development

built basic "Hello world!" Py app as to ensure virtual enviroment was working corretly.
http://127.0.0.1:5000/ (local host) shows "Hello World!". 
Render onto HTML file. 

I want to make use of Bootstrap, its ability to make impressive CSS that is adaptive to screensizes ect. 
made it a perfect choise to ensure my apps style is consistant and clean. 

Using the "starter template" (https://getbootstrap.com/docs/5.0/getting-started/introduction/)
 
img logo
https://drive.google.com/open?id=1EZtluKS1qXB-IYiJIcFL-CavCokCp12e (still not working needs static folder)

Created base website with navigation bar (in base.html), using the {% block content %} and {% end block %} 
flask functions I was able to create a template for the other pages of the site. The header and meta data needed
for the browser to interprate the information is placed in every page along with the js <scripts> needed to run the site,
the closing tags are also included as to not get syntax errors.

For added efficiency I have made use of Jinja2 to create a more dy namic website. 
sing the flask templateing language I can use its logic to update page names and veriables from my app.py

@app.route('/')
def index():
    title = "The Paper Folk"
    return render_template("index.html", title=title)

This basic function allows me to change the titles from the app.py dynamicly. 

Added MongoDB support, login form submits username and password to cluster. 

issues with encrypting: password is encrypting
wont de-cypt when loggin in. posts to dashboard without this method. 






  

