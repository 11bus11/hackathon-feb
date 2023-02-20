# Helping Hands
This project was made during the "Hackathon-Feb-2023: *World NGO Day February 27th*" at Code Institute.

## Team Name: <<team_name>>
​
[Link to Deployed Project](https://helping-hand-ci.herokuapp.com)
​
## Contents(#contents)
​
* [User Experience (UX)](#user-experience)
  * [User Stories](#user-stories)
* [Technology](#technology)
* [Design](#design)
  * [Color Scheme](#color-scheme)
  * [Typography](#typography)
  * [Imagery](#imagery)
  * [Wireframes](#wireframes)
* [Deployment & Usage](#deployment)
* [Testing](#testing)
* [Credits](#credits)
  * [Code](#code)
  * [Content](#content)
  * [Media](#media)
  * [Acknowledgements](#acknowledgements)
​
## User Experience
We wanted to cater to users wondering how they can help and/or donate to NGOs.
​
### User stories
We wanted the user to:
* Find NGOs they can donate to.
* Find events they can take part in.
* See what each featured organisation does.
* Navigate the website easily.

We wanted the admin to:
* Be able to add, delete or change the featured organisations.
* Be able to add, delete or change the events on the website.
​
## Technology

### Requirements
```
asgiref==3.5.2
chardet==3.0.4
click==8.1.3
dj-database-url==0.5.0
Django==3.2.16
django-allauth==0.41.0
gunicorn==20.1.0
idna==2.8
itsdangerous==2.1.2
oauthlib==3.1.1
psycopg2==2.9.5
psycopg2-binary==2.9.5
python3-openid==3.2.0
pytz==2022.6
requests==2.22.0
requests-oauthlib==1.3.0
sqlparse==0.4.3
urllib3==1.25.11
Werkzeug==2.2.2
whitenoise==6.3.0
```
​
### Languages
* HTML
* CSS
* JavaScript
* Python

​
### Tools & Frameworks
* Bootstrap - Used for styling
* Django - Used for backend
* PostgreSQL - Used for the database. The database is hosted on [ElephantSQL](https://www.elephantsql.com/)
​
## Initial MVP idea:
​
Our idea started out as a simple website for finding NGOs. When we were done discussing it, we had a home page, an event page, a donation page, and a socials page. We also had a search bar.
​
## Actual idea & content:
​
At the end we made the socials page and donate page into a single page. We also removed the search bar due to comming to the conclution that we would not have the time. We also developed the way the navigation looked.

That means that the website has these pages:
### Home page
The home page has information about World NGO Day and how people can support NGOs. It also links to the donate page and a carucel with images linked to different NGOs.

### Donate page
Most of this page is taken up by a list of different NGOs. Each item in the list has information about the organisation and an image with their logo. At the bottom there is links to their website, and social media if they have one. Above the list there is also some general information on how people contribute to NGOs. 

The information about each NGO is stored in a database, which makes it easy to edit, delete or add organisations.

### Event page
This page has some events people can attend. There is a smaller navigation bar right above the list of events. This contains all the locations (what country the event is in). The list below contains basic information about the event, and a link to the events official page. 

The information about each NGO is stored in a database, which makes it easy to edit, delete or add events. This is especially useful, since the events need to be deleted from the website after taking place.

Other features:
### Navigation
The navigation consists of a navigation bar on the right and the sites logo on the left. The logo liks to the home page, and the three different items in the navbar links to the pages shown above (home, donate, events). The text is white on an orange background.

### Footer
​The footer has links to social media and copywrite information. Here too, the text is white on an orange background.
​
## Design
​
### Color Scheme
<< detail your color palette here >>
We chose an orange and white colour palette. These colours are often used in similar pages, and work well with our layout ideas.
​
### Typography
<< what font pairings did your team consider and pick? And why? >>
We chose Helvetica due to it being the one used on the WorldNGO website. To make the two websites feel connected, we too chose to use it. It is also san serif, which is easier to read on screans than serif fonts. 
​
### Imagery
<< Detail imagery used to compliment your build & theme >>
We have a hero image, and logos for the different organisations. The logos are used in the list of featured organisations. It helps people to recognize the different NGOs.
​
<< ensure source attribution is maintained, and that you have used copyright-free material >>
​
### Wireframes and mockups
​
#### Wireframes
![home](media/documents/wf-home.png)
![events](media/documents/wf-events.png)
![donate](media/documents/wf-donate.png)

#### Mockups
![donate](media/documents/mockup-donations-page.jpg)
![home 1](media/documents/mockup-home-1.png)
![home 2](media/documents/mockup-home-2.png)
![home 3](media/documents/mockup-home-3.png)
![home 4](media/documents/mockup-home-4.png)
​
​
## Deployment
This project was deployed with Heroku, and used Whitenoise for its static files.

* Create an account at Heroku, and do not forget you need to confirm your e-mail to do this.
* Create a list of dependencies in a text file named requirements (pip3 freeze > requirements.txt).
* Create an app by clicking the "create a new app" button found on the dashboard.
    * Choose a unique app name.
    * Choose your region and click "create app"
* Click on settings (for the app).
    * Find the Config Vars section and add potential files that you cannot upload to github. For example API credentials. KEY is the title, and VALUE is the content. For thos project you need to add the Django key and the database-url.
    * Add buildpacks (below Config Vars). For this project, I installed Python and Node.js. Make sure they are in the correct order.
* Go to the deploy section.
    * Choose to deploy from GitHub.
    * Connect your account and choose a repository to deploy from.
    * Choose either Automatic or Manual deployment (recommended).
* Follow the steps on this page to set up Whitenoice. This is the same instructions I used. Dont forget to run the command "python3 manage.py collectstatic".
* Make sure your images are on an external site, like ibb. This prevents errors related to the images.
* Make sure the live site is working.

​
## Testing

### User stories testing
We wanted the user to:
* Find NGOs they can donate to.
    * These can be found on the donate page.
* Find events they can take part in.
    * These can be found on the events page.
* See what each featured organisation does.
    * The organisation summary explaines what each organisation does.
* Navigate the website easily.
    * There is a navbar at the top of the website. It is in the same position regardless of what page you are on.

We wanted the admin to:
* Be able to add, delete or change the featured organisations.
    * This can be done on the [admin page]()
* Be able to add, delete or change the events on the website.
    * This can be done on the [admin page]()

### Device testing
This website was tested natively on these devices:
- Desktop Computer (25" screen)
- Acer Aspire 5 (15" screen)

It was also tested on these devices with Mozilla- and Google dev tools:


### Browser testing
This website was tested on the following browsers:
* Mozilla Firefox
* Google Crome
* Microsoft Edge
* Safari
* DuckDuckGo (mobile)

### Validator testing

* HTML - I put the HTML documents through the w3c validator. It did not return any errors not related to the use of django.
* CSS - 
* Python - I put the code through the Code Institute [pep8 linter](https://pep8ci.herokuapp.com/). Got no errors exept "line to long".
* JavaScript - I ran the JavaScript through the [JS validator](https://jsvalidator.com/) and got no errors.

![JS validator result](media/documents/js-validator.JPG)

### Lighthouse

### Manual Testing
* We tested if the data from the backend showed up correctly by asking the page to show it. 
* We did the testing of the images link in a similar way. When the name of the image-file had been added, we checked if it showed up in the frontend. If it did not, we inspected the page and checked what the link looked like in reality. That helped us find the problems.

### Bugs

#### Fixed bugs
* At first the logo images for the organisations did not show up. This was due to us having accidentally added an extra slash. To figure this out we inspected the page in the browser.

#### Unfixed bugs​
* The body does not fill the whole page. There is a small part on the top of the page where the body tag does not reach.

## Credits
​
### Code
<< any and all code that isn't yours...must go here >>

​
### Content
<< any content, such as facts/references/text that isn't yours...must go here >>
The organisation and event summaries are taken from the organisations websites. These can be found on the page right below the summary.

The deployment part of the readme is the same as in Erik's (team-member) [Project 4](https://github.com/11bus11/theatre-booking).
​
### Media
<< you may have already done this above in the Imagery section, but just in case, please attribute Media acquisition here >>

​
### Acknowledgements
* [Erik Vodopivec Forsman](https://www.linkedin.com/in/erik-vodopivec-forsman-485b61217)
* [James Kasetarapanya](https://www.linkedin.com/in/james-kasetarapanya-86602585/)
* [Russell Stanley Smith](https://www.linkedin.com/in/russellstanleysmith/)
* [Jack Crosbie](https://www.linkedin.com/in/jack-crosbie-27770224a/)
