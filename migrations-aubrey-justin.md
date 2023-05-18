Setup
Create a new Rails application called 'favorite_movies'.✅
Create the database✅
Generate a Movie model with a title attribute and a category attribute✅


Challenges
Add five entries to the database via the Rails console✅

Create a migration to add a new column to the database called movie_length✅

take one:
rails db:migrate
== 20230518223146 AddColumnMovieLengthToMovie: migrating ======================
-- add_column(:lists, :item, :string)
rails aborted!
StandardError: An error has occurred, this and all later migrations canceled:

PG::UndefinedTable: ERROR:  relation "lists" does not exist
/Users/learnacademy/Desktop/migrations-ad-jk/db/migrate/20230518223146_add_column_movie_length_to_movie.rb:3:in `change'

Caused by:
ActiveRecord::StatementInvalid: PG::UndefinedTable: ERROR:  relation "lists" does not exist
/Users/learnacademy/Desktop/migrations-ad-jk/db/migrate/20230518223146_add_column_movie_length_to_movie.rb:3:in `change'

Caused by:
PG::UndefinedTable: ERROR:  relation "lists" does not exist
/Users/learnacademy/Desktop/migrations-ad-jk/db/migrate/20230518223146_add_column_movie_length_to_movie.rb:3:in `change'
Tasks: TOP => db:migrate
(See full trace by running task with --trace)

correct way:
class AddColumnMovieLengthToMovie < ActiveRecord::Migration[7.0]
 
  def change
    add_column :movies, :movie_length, :string
  end
end


Update the values of the five existing attributes to include a movie_length value


Generate a migration to rename the column 'category' to 'genre'