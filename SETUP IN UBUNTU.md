## How To Setup CircuitVerse on Ubuntu [Quickstart]

### Introduction
CircuitVerse is a web-based simulation software for creating and testing digital circuits. 
The easy drag and drop feature makes it easier and a fun way to learn about logic circuits and also compatible to be used by teachers as well as students.
From simple gates to complex sequential circuits, plot timing diagrams, automatic circuit generation, explore standard ICs, and much more, CircuitVerse has got you covered.
It also lets the user store and access the previously built circuits to build yet more complex circuits and generate truth tables for the constructed circuits

![CircuitVerse Logo](https://github.com/CircuitVerse/CircuitVerse/raw/master/public/img/cvlogo.svg?sanitize=true)

This tutorial will walk you through setting up and configuring the development environment for [CircuitVerse](https://circuitverse.org/) on an Ubuntu server. 
For a more detailed version of this tutorial, with better explanations of each step, please read along.

***

### Pre-requitses
- Ubuntu 18.04 or above
- Git 2.26.2 Installed [Tutorial](https://www.digitalocean.com/community/tutorials/how-to-install-git-on-ubuntu-18-04-quickstart)
- Ruby Version: ruby-2.6.5 [Tutorial](https://www.digitalocean.com/community/tutorials/how-to-install-ruby-and-set-up-a-local-programming-environment-on-ubuntu-16-04)
- Rails Version: Rails 6.0.1 [Tutorial](https://www.digitalocean.com/community/tutorials/how-to-install-ruby-on-rails-with-rbenv-on-ubuntu-18-04)
- PostgreSQL Version: 9.5 [Tutorial](https://www.digitalocean.com/community/tutorials/how-to-install-and-use-postgresql-on-ubuntu-18-04)
- Yarn [Tutorial](https://linuxize.com/post/how-to-install-yarn-on-ubuntu-18-04/)
- Docker [Tutorial](https://www.digitalocean.com/community/tutorials/how-to-install-and-use-docker-on-ubuntu-18-04)
- Redis [Tutorial](https://www.digitalocean.com/community/tutorials/how-to-install-and-secure-redis-on-ubuntu-18-04)
- Imagemagick [Tutorial](https://linuxconfig.org/how-to-install-imagemagick-7-on-ubuntu-18-04-linux)
***

## Step 1 — Fork From CircuitVerse
To contribute, first fork 🍽️ the original repository by navigating at the top of the repository in GitHub.

![fork](https://user-images.githubusercontent.com/42115530/81844206-5c8d6b80-956c-11ea-998d-beac8ee1468d.png)

## Step 2 — Clone the repo
Clone the forked repository into your local machine using the following command:
```
$ git clone https://github.com/your-username/CircuitVerse.git
$ cd CircuitVerse
```
You can copy the URL by using the green “Clone or download” button from your repository page that you just forked from the original repository page. Once you click the button, you’ll be able to copy the URL by clicking the binder button next to the URL:

![clone](https://user-images.githubusercontent.com/42115530/81844918-6ebbd980-956d-11ea-855a-87cff1a6bfbf.png)

## Step 3 — Install dependencies

```
$ bundle install
```
You might get an error stating:
```
An error occured while installing pg (1.1.4), and Bundler cannot continue.
Make sure that `gem install pg -v '1.1.4' --source 'https://rubygems.org/' succeeds before bundling.

In Gemfile:
pg
```

To run it correctly, try this:
```
$ sudo apt-get install postgresql
$ sudo apt-get install libpq-dev
```
Then
```
$ gem install pg
```
then
```
$ bundle install
```

## Step 4 — Configure your PostgreSQL database
Copy `config/database.example.yml` and paste into `config/database.yml` and update the Postgres credentials need to be updated to your currently running database.

!](https://user-images.githubusercontent.com/42115530/81856035-ceba7c00-957d-11ea-8aa8-5eef7233f1c1.PNG)

## NOTE:
Make sure you have updated the username and password to your postgres username and password as shown below.
```
  username: 'yourusername'
  password: 'yourpassword'
```

![rails db](https://user-images.githubusercontent.com/42115530/81952842-928e2680-9624-11ea-86c1-f11611eccbfa.PNG)


## Step 5 — Create Database
```
$ rails db:create
```
You might get an error stating `rails aborted`, so, try this:
```
$ sudo apt-get install nodejs 
```
or
```
$sudo npm install --global yarn
```

## Step 6 — Run Migrations
```
$ rails db:migrate
```
