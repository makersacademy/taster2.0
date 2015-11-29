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

What we will do now is Forking the project. That means, doing a copy of someone repo into your own profile. That will allow you to have a proper copy of the project where you can work easily and do a "pull request" if you are satisfate with your work. The pull request will send a notification to the project owner. He will be able to check your code and if he likes it, then incorporate it inside his project.

1- Go to the [GitHub project page](https://github.com/BobRazoswki/Taster-Challenge_4 "taster challenge 4")
2- Click on "Fork"                                                 
![fork](https://raw.githubusercontent.com/makersacademy/taster2.0/master/assets/images/CSS%20Challenge/fork.png)

3- Wait during the progress                                                 
![waiting process](https://raw.githubusercontent.com/makersacademy/taster2.0/master/assets/images/CSS%20Challenge/wait.png)

4- You can now see it on your profile                                                 
![forked repo](https://raw.githubusercontent.com/makersacademy/taster2.0/master/assets/images/CSS%20Challenge/forked.jpg)


5- Clone the project inside your computer                                                 

Be careful, cloning a project will directly create the repo with its name.                                                           
So run the command where you want to see your project folder (something easy, like your desktop)

```bash
git clone https://github.com/BobRazoswki/Taster-Challenge_4.git
cd Taster-Challenge_4
atom .
```
> cd stands for change directory, it is the way to go from one folder to an another one inside of the terminal
> atom . Will open everything inside the repo on atom (that's what the " . " is for)
If you prefer, you can open your text editor and open the project via File > open >

6- Today, only two files will interest us:                                                 
  - Index.erb
  - Style.css

**You can find them in: app > views > index.erb && public > css > style.css**

I let you find out and explore a bit what is happening in the different files.
> After the course, feel free to modify them and have fun to play with it in order to understand how it is working !


7- In order to see the project live, you will need to start the server with:                                                 

```bash
Open a new tab in your terminal with cmd + t
heroku local
```

8- Just to see if it is working:                                                 
  - Write a Hello World in your index.html
  - Open your browser
  - Go on this URI: http://localhost:5000

If it is working, go on the next step !

9- Once you've coded your first feature you can push it live to see if Heroku server interpret exactly the same thing as your local server (heroku local).

Remember, if you are agile, you release **often** and **early** ! So do it after each features.

to do that run the following commands :

```bash
heroku create the-name-of-your-project
git add .
git commit -m "adds my first feature"
git push origin master
git push heroku master
heroku open
```
###Section 3 -  Create a new page !

Let's sum it up a bit.

1- You already know how to code HTML and CSS, put them together in order to have a beautiful website.                  
2- You know how to load a library in order to use already build features.                                              
3- You know how to push it properly on your local machine and on Heroku.                                                 

Now, let's create our second page and link it to the first one.

1- Create a second file in /views (name it as you want).                                                 
2- Open the index.rb inside /controllers and make a GET request to the new page you've just created.

```ruby
get '/my-second-page' do
  erb :my-second-page
end
```

3- You can now code inside the my-second-page.erb and you will see the changement if you go to:                         
  - http://localhost:5000/my-second-page (to see the changement locally)
  - http://my-application.herokuapp.com  (after having pushed it to github)

4- You can know link your different pages inside your menu :)                                                       
5- Try to make your page responsive

> If you think you are not ready for responsive, no worries, we can wait to have strong basis and after jump on Responsive.

You can now go code and push it live every time you get something done.
