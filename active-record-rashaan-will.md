Add five family members into the Person table in the Rails console.
 Person.create(first_name: 'Jack', last_name: 'Bowen', phone: '000-000-0003')
  #<Person:0x000000010cd9bcc0 id: 3, first_name: "Jack", last_name: "Bowen", phone: "000-000-0003", created_at: Thu, 18 May 2023 17:45:37.379858000 UTC +00:00, updated_at: Thu, 18 May 2023 17:45:37.379858000 UTC +00:00>,

Retrieve all the items in the database.
 Person.all

[#<Person:0x000000010cd9bf40 id: 1, first_name: "Ellie", last_name: "Hamilton", phone: "000-000-0001", created_at: Thu, 18 May 2023 17:44:16.039025000 UTC +00:00, updated_at: Thu, 18 May 2023 17:44:16.039025000 UTC +00:00>,
 #<Person:0x000000010cd9be00 id: 2, first_name: "Hank", last_name: "Bowen", phone: "000-000-0002", created_at: Thu, 18 May 2023 17:45:26.627856000 UTC +00:00, updated_at: Thu, 18 May 2023 17:45:26.627856000 UTC +00:00>,
 #<Person:0x000000010cd9bcc0 id: 3, first_name: "Jack", last_name: "Bowen", phone: "000-000-0003", created_at: Thu, 18 May 2023 17:45:37.379858000 UTC +00:00, updated_at: Thu, 18 May 2023 17:45:37.379858000 UTC +00:00>,
 #<Person:0x000000010cd9bb80 id: 4, first_name: "Mike", last_name: "Bowen", phone: "000-000-0004", created_at: Thu, 18 May 2023 17:45:49.986463000 UTC +00:00, updated_at: Thu, 18 May 2023 17:45:49.986463000 UTC +00:00>,
 #<Person:0x000000010cd9ba40 id: 5, first_name: "Pat", last_name: "Bowen", phone: "000-000-0005", created_at: Thu, 18 May 2023 17:46:00.073966000 UTC +00:00, updated_at: Thu, 18 May 2023 17:46:00.073966000 UTC +00:00>] 

Add yourself to the Person table.
Person.create(first_name: 'Will', last_name: 'Bowen', phone: '000-000-0006')
#<Person:0x000000010cd3fc90 id: 6, first_name: "Will", last_name: "Bowen", phone: "000-000-0006", created_at: Thu, 18 May 2023 17:47:46.171513000 UTC +00:00, updated_at: Thu, 18 May 2023 17:47:46.171513000 UTC +00:00> 

Retrieve all the entries that have the same last_name as you.
Update the phone number of the last entry in the database.
Retrieve the first_name of the third Person in the database.