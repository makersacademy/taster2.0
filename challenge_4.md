Challenge 4 - You first project !
================

###Section 1 -  Link a library (30min)

In order to stick the task to your memory, let's do it !

For this project, we will use the Twitter Bootstrap Library.

In order to link it, you can:
  1- Download the library
    - Link it from your assets to your index file.
  2- Load it from a Content Delivery Network (CDN)
    - It is quick to do, and loads faster because it comes from an another server, so while yours is loading the content, the CDN is loading the library.

> The best practice will be to load both:                                                                               
Load the CDN, if the CDN is not available, then, load the local library                                               
I let you explore how to do that ;)

###Section 2 -  The big settlement !

1- Open your terminal
2- Clone the project from github:

```bash
git clone git@github.com:BobRazoswki/test-taster.git
```
3- Open the project with your text editor
4- In order to see the project live, you will need to start the server with:

```bash
cd /the root path of your repository
heroku local
```

5- Today, only two files will interest us:
  - Index.erb
  - Style.css

**You can find them in: app > views > index.erb && public > css > style.css**

I let you find out and explore a bit what is happening in the different files.
> After the course, feel free to modify them and have fun to play with it in order to understand how it is working !

6- Just to see if it is working:
  - Write a Hello World in your index.html
  - Open your browser
  - Go on this URI: http://localhost:5000

If it is working, go on the next step !

7- Once you've coded your first feature you can push it live to see if Heroku server interpret exactly the same thing as your local server (heroku local).

Remember, if you are agile, you release **often** and **early** ! So do it after each features.

to do that run the following commands :

```bash
heroku create the-name-of-your-project
git add .
git commit -m "adds my first feature"
git push origin master && git push heroku master
heroku open
```
###Section 3 -  Make it ! (the rest of the day, and more ;) )

Yesterday you prepared all the material to be ready for coding.

We've seen the step you should take before coding.

Let's sum them up quickly:

1- Think about the project and write a correct descriptive.                                        
  - Talk about it with your pair                                        
  - Defines what it will do, for who, how, etc.                                        
2- Start writing user stories and user scenarios.                                        
3- Draw the Mockups in order to not forget anything and to be as clear as possible with your team.                      
4- Think the architecture of your website, write it on paper.                                        
5- Think how you will display the element, their position, and think about the Responsiveness of it.                                        
> If you think you are not ready for responsive, no worries, we can wait to have strong basis and after jump on Responsive.
