# Linux Server Configuration

## Ip Address
```
52.88.108.116
```

## SSH 
```
ssh -p 2200 -i [RSA_FILE] grader@52.88.108.116
```
## Installed Software
###Udacity Item Catalog
This is an application that provides a list of items within a variety of categories as well as provide a user registration and authentication system. Registered users will have the ability to post, edit and delete their own items.

###Changes made
-Changed database to Postgres
```
engine = create_engine("postgresql://catalog:[password]@localhost/restaurant")
```

-Moved files to /usr/share/catalog

-Created psql database user catalog and assigned to database restaurant

-Created a wsgi file to run the application

-Configured Apache to load the app when the root web directory is accessed online

## Third-party resources used
-finger
-fail2ban
-cron-apt
-Glances 
