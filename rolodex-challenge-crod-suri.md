Challenge: Rolodex

As a developer, I have been tasked with creating a database model that will be used in a rolodex application. I want to ensure that the database behaves as expected and the necessary actions can be performed on the database instances.

Set Up

##Create a new Rails app named 'rolodex_challenge'.

rails new rolodex-challenge -d postgresql -T

cd rolodex-challenge 

##Create the database. The output in the terminal should look like this:

rails db:create

// Created database 'rolodex_challenge_development'
//Created database 'rolodex_challenge_test'

Created database 'rolodex_development'
Created database 'rolodex_test'

##Generate a model called Person with a first_name, last_name, and phone. All fields should be strings.

rails generate model Person first_name:string last_name:string phone:string

##Run a migration to set up the database.

rails db:migrate

##Open up Rails console.

rails c


#Actions

##Add five family members into the Person table in the Rails console.

Person.create(first_name: "Summer", last_name: "Smith", phone: "3176786892")
Person.create(first_name: "Suri", last_name: "Rodriguez", phone: "1234567891")
Person.create(first_name: "Spongebob", last_name: "Squarepants", phone: "1234567868")
Person.create(first_name: "Rick", last_name: "Sanchez", phone: "3176781234")
Person.create(first_name: "Morty", last_name: "Smith", phone: "3176783456")

##Retrieve all the items in the database.

Person.all

##Add yourself to the Person table.

Person.create(first_name: "Catalino", last_name: "Rodriguez", phone: "4438668011")

##Retrieve all the entries that have the same last_name as you.

Person.where(last_name: "Rodriguez")

##Update the phone number of the last entry in the database.

y=Person.last
y.update(phone: "1235467890")

##Retrieve the first_name of the third Person in the database.

thirdperson = Person.select(:first_name)
thirdperson.find(3)


#Stretch Challenges

##Update all the family members with the same last_name as you, to have the same phone number as you.

updatephone = Person.where(last_name: "Rodriguez")
updatephone.update(phone: "4438668011")

Remove all family members that do not have your last_name.

notlastname = Person.where.not(last_name:  "Rodriguez")
notlastname.destroy_all