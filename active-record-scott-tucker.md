As a developer, I have been tasked with creating a database model that will be used in a rolodex application. I want to ensure that the database behaves as expected and the necessary actions can be performed on the database instances.

Set Up

Create a new Rails app named 'rolodex_challenge'. DONE


Create the database. The output in the terminal should look like this: 
Created database 'rolodex_development'
Created database 'rolodex_test' DONE


Generate a model called Person with a first_name, last_name, and phone. All fields should be strings.
rails generate model 'rolodex_challenge' first_name:string last_name:string phone_number:string

Run a migration to set up the database.
DONE

Open up Rails console.
DONE

Actions

Add five family members into the Person table in the Rails console.

SCOTT 5 FAMILY MEMBERS
RolodexChallenge.create first_name:, last_name:, phone_number:

Retrieve all the items in the database.
RolodexChallenge.all

Add yourself to the Person table.
RolodexChallenge.creat first_name:'Scott', last_name:'Stark', phone_number:'555-5556'

Retrieve all the entries that have the same last_name as you.
RolodexChallenge.where last_name:'Stark'

Update the phone number of the last entry in the database.
RolodexChallenge.find 6 --> cell.phone_number = '555-5557' --> cell.save


Retrieve the first_name of the third Person in the database.
RolodexChallenge.find(3).first_name 

Stretch Challenges

Update all the family members with the same last_name as you, to have the same phone number as you.
Remove all family members that do not have your last_name.