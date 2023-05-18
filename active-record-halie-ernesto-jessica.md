Challenge: Rolodex
As a developer, I have been tasked with creating a database model that will be used in a rolodex application. I want to ensure that the database behaves as expected and the necessary actions can be performed on the database instances.
Set Up

* Create the database. The output in the terminal should look like this:
Created database 'rolodex_development'
Created database 'rolodex_test'

* Generate a model called Person with a first_name, last_name, and phone. All fields should be strings.
* Run a migration to set up the database.
* Open up Rails console.
Actions
* Add five family members into the Person table in the Rails console.
* Retrieve all the items in the database.
* Add yourself to the Person table.
* Retrieve all the entries that have the same last_name as you.
* Update the phone number of the last entry in the database.
* Retrieve the first_name of the third Person in the database.


Stretch Challenges
* Update all the family members with the same last_name as you, to have the same phone number as you.
```If you have more than 1 object saved in a new variable and you want to modify all the objects in the new variable - you must use the .update()```

* Remove all family members that do not have your last_name.
```If you have more than 1 object saves in a new variable and you want to delete all of the objects in the new varialbe - you must use the .destroy_all```