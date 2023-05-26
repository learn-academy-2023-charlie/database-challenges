

Setup
Create a new Rails application called 'favorite_movies'.

rails new favorite_movies -d postgresql -T

Create the database

rails db:create

Generate a Movie model with a title attribute and a category attribute

rails g model Movie title:string category:string

Challenges
Add five entries to the database via the Rails console

Movie.create(title: 'The Last Samurai', category: 'Action, Drama')
Movie.create(title: 'The Avengers', category: 'Action, Comedy')
Movie.create(title: 'Eyes Wide Shut', category: 'Suspense')
Movie.create(title: 'Cars', category: 'Kids')
Movie.create(title: 'Transformers', category: 'Action')

Create a migration to add a new column to the database called movie_length

rails generate migration add_column

Update the values of the five existing attributes to include a movie_length value

Movie.find(1).update(movie_length: '60 min')
Movie.find(3).update(movie_length: '80 min')
Movie.find(4).update(movie_length: '75 min')
Movie.find(5).update(movie_length: '85 min')
Movie.find(6).update(movie_length: '65 min')

Generate a migration to rename the column 'category' to 'genre'

rails g migration rename_column

rename_column :movies, :category, :genre   ---- in migration file

rails db:create