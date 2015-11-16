Pre course
================

Before writing your first line of code, you need to install many many things.
Let's sum them up quickly:

- Git (For version control, team work, remote, etc)
- Github (To have a visual platform of git and much much more)
- Ruby (Our OOP language)
- Heroku (The company that will host our website for us)
- A text editor ([Atom](https://atom.io/ "Atom.io") or [Sublime Text  3](https://www.sublimetext.com/3 "Sublime text 3"))

This is definitly not an exhaustive list, but it will be enough for the Taster weekend

####On MAC and Windows
1- Create an account on [Github](https://github.com/join "Github")                                            
2- Create an account on [Heroku](https://signup.heroku.com/ "Heroku")                                                   
3- Download and install the **right** heroku toolbelt for your OS on [Heroku Toolbelt](https://toolbelt.heroku.com/                                         "Heroku toolbelt")

>The toolbelt is a set of few things that you will to develop.
it has Heroku command line + Git and ruby

4- Restart your computer                                                                  
5- Open your terminal and run:                                                                  

>The " $ " sign is the line you need to write (don't write it), the other lines are the terminal answers

>You will never see the bullet points while you are typing your password in the terminal.

```bash
$ heroku login
Enter your Heroku credentials.
Email: me@example.com
Password:

$ cd && cat .netrc
machine api.heroku.com
  login me@example.com
  password c4cd94da15ea0544802c2cfd5ec4ead324327430
machine git.heroku.com
  login me@example.com
  password c4cd94da15ea0544802c2cfd5ec4ead324327430
```

On Mac
================

You will need to go trough this website:
http://preparetocode.io follow the essential tools path

On Windows
================

You will need to install few things
- http://scoop.sh/
- https://github.com/ConradIrwin/pry-windows
