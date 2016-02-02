# Week 06

### Question 1

You're working on your Tunr app and you encounter this error. What does it mean and where would you go first to address it?  

![Rails error](http://i.imgur.com/9NR7XNT.png)  

```text
I am missing a view for my Artist controller's index action. I would remedy that by creating an `index.html.erb` inside of the `views/artists` directory.
```

### Question 2

What is the difference between...  
• Creating a migration to add a column   
• Editing an existing migration and running `rake db:migrate:reset`   

```text
Creating a migration to add a column adds a column to an already-existing table in a database. Editing an existing migration and running rake db:migrate:reset wipes the entire database and rebuilds it using existing migrations, including the newly-edited one.
```

### Question 3

In a Rails application, how is the router related to controller actions?  

```text
A router will direct a user to a particular controller action depending on the content of the incoming HTTP request.
```

### Question 4

Assuming our Tunr Rails app (1) has a Song model that belongs to an Artist model and (2) uses nested resources, what is the path helper for `songs#new`? (Select one answer)  

1. `artist_song_path( @artist, @song )`  
2. `new_artist_song_path( @artist )`  
3. `create_artist_song_path( @artist )`  
4. `new_artist_song_path( @artist, @song )`  
5. `new_song_path( @song )`  

```text
4. new_artist_song_path( @artist, @song )
```

### Question 5

Where are (a) cookies and (b) session variables stored? (Select one answer)  

1. (a) Server, (b) Browser  
2. (a) Browser, (b) Database  
3. (a) Database, (b) Server  
4. (a) Browswer, (b) Server  

```text
4. (a) Browser, (b) Server
```

### Question 6

The Rails asset pipeline manages which of the following... (Select all answers that apply)

1. Stylesheets  
2. Javascript files  
3. Gems  
4. Images  
5. API keys  
6. Usernames and passwords  

```text
1. Stylesheets
2. Javascript files
4. Images
```

### Question 7

What is the correct way to run a migration on Heroku?  

1. `rake db:migrate`  
2. `heroku rake db:migrate`  
3. `heroku run db:migrate`  
4. `heroku run rake db:migrate`  
5. `heroku db:migrate`  

```text
4. heroku run rake db:migrate
```
