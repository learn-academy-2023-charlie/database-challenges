# Create rails framework remove sql lite and replace with postgres
    $ rails new rolodex_challenge -d postgresql -T

# Cd to repo
    $ cd rolodex_challenge

# Create Database
    $  rails db:create

# Create model (Columns, rows,etc...)
    $  rails generate model Person first_name:string last_name:string phone:string

# Start server to show everything is working. Will get migration error.
    $ rails server

# Begin Migration
    $ rails db:migrate

# Open Rails terminal to interact with database
    $ rails c

# Challenge: Rolodex
As a developer, I have been tasked with creating a database model that will be used in a rolodex application. I want to ensure that the database behaves as expected and the necessary actions can be performed on the database instances.

Set Up

Create a new Rails app named 'rolodex_challenge'. ✅
Create the database. The output in the terminal should look like this:✅
Created database 'rolodex_development'
Created database 'rolodex_test'
Generate a model called Person with a first_name, last_name, and phone. All fields should be strings.✅
Run a migration to set up the database.✅
Open up Rails console.✅
Actions

Add five family members into the Person table in the Rails console.✅
# Person.create first_name:"Easter", last_name:"Bunny", phone:"1-444-500-6000"
Retrieve all the items in the database.✅
# Person.all
Add yourself to the Person table.✅
# Person.create first_name:"Easter", last_name:"Bunny", phone:"1-444-500-6000"
Retrieve all the entries that have the same last_name as you.✅
# Person.where last_name:"Clause"
Update the phone number of the last entry in the database.

Retrieve the first_name of the third Person in the database.
Stretch Challenges

Update all the family members with the same last_name as you, to have the same phone number as you.
Remove all family members that do not have your last_name.