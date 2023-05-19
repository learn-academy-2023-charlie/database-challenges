<!-- Challenge: Rolodex
As a developer, I have been tasked with creating a database model that will be used in a rolodex application. I want to ensure that the database behaves as expected and the necessary actions can be performed on the database instances.

Set Up

Create a new Rails app named 'rolodex_challenge'.

    rails new rolodex_challenge -d postgresql -T


Create the database. The output in the terminal should look like this:
Created database 'rolodex_development'
Created database 'rolodex_test'

    rails db:create

Generate a model called Person with a first_name, last_name, and phone. All fields should be strings.

    rails generate model Person first_name:string last_name:string phone:string

Run a migration to set up the database.

    rails db:migrate

Open up Rails console.

    rails c

Actions

Add five family members into the Person table in the Rails console.
    
    Person.create(first_name: 'Yue Hen', last_name: 'Lee', phone: '123-456-789') X 5

Retrieve all the items in the database.

    Person.all

Add yourself to the Person table.

    Done already

Retrieve all the entries that have the same last_name as you.

    Person.where(last_name: 'Lee'

Update the phone number of the last entry in the database.

    Person.last.update(phone: '987-654-321')

Retrieve the first_name of the third Person in the database.

    Person.find(3)

Stretch Challenges

Update all the family members with the same last_name as you, to have the same phone number as you.

    Person.where(last_name: 'Lee').update(phone: '123-456-789')

Remove all family members that do not have your last_name.

    Person.where.not(last_name:'Lee').destroy_all

 -->

    