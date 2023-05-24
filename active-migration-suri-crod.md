Challenges

#Add five entries to the database via the Rails console


    Movie.create(title: "Interstellar", category: "Sci-Fi")
    Movie.create(title: "Jurassic Park", category: "Sci-Fi")
    Movie.create(title: "Super Mario Bros", category: "Animation")
    Movie.create(title: "Up!", category: "Animation")
    Movie.create(title: "Fast X", category: "Action")


#Create a migration to add a new column to the database called movie_length

    exit

    rails g migration add_column_movie_length_to_movie

    class AddColumnMovieLengthToMovie < ActiveRecord::Migration[7.0]
    def change
        add_column :movies, :movie_length, :string
    end
    end

    rails db:migrate

#Update the values of the five existing attributes to include a movie_length value 

    Movie.last.update(movie_length: "1 hr, 40 min")
    Movie.fourth.update(movie_length: "2 hr, 20 min")
    Movie.third.update(movie_length: "3 hr, 2 min")
    second = Movie.find 2
    second.update(movie_length: "1hr, 30 min")
    first = Movie.find 1
    first.update(movie_length: "2 hr, 5 min")


#Generate a migration to rename the column 'category' to 'genre'

    exit

    rails g migration change_column_category_to_genre

    