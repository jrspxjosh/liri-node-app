# liri-node-app

Technologies Utilized: Node.js, Spotify API, Twitter API, OMDB API, and File Support for reading and writing to a log.txt

L.I.R.I. stands for Language Interpretation and Recognition Interface. LIRI is like iPhone's SIRI. However, while SIRI is a Speech Interpretation and Recognition Interface, LIRI is a Language Interpretation and Recognition Interface. LIRI is a command line Node app that takes in parameters and gives you back data.

As the name suggests, LIRI is analagous to the iPhone's SIRI assistant, but rather than using speech, LIRI is controlled through written text.

The LIRI app uses Node.js in the command line of your computer and has dependencies for the request, spotify, and twitter Node packages. It also used the built-in fs package to read and write to text files.

The app features 4 different features using the node liri.js [command-here] syntax. Below are the command types...

What Each Command Should Do

Twitter

node liri.js my-tweets
my-tweets returns your Twitter account's 20 most recent tweets using the Twitter API.


Spotify

node liri.js spotify-this-song '<song name here>'

You will utilize the node-spotify-api package in order to retrieve song information from the Spotify API.

This will show the following information about the song in your terminal/bash window using the Spotify API.

Artist(s)
The song's name
A preview link of the song from Spotify
The album that the song is from.

If no song is provided then your program will default to "The Sign" by Ace of Base.


IMDb

node liri.js movie-this '<movie name here>'

This will output the following information to your terminal/bash window:

  * Title of the movie.
  * Year the movie came out.
  * IMDB Rating of the movie.
  * Rotten Tomatoes Rating of the movie.
  * Country where the movie was produced.
  * Language of the movie.
  * Plot of the movie.
  * Actors in the movie.

If the user doesn't type a movie in, the program will output data for the movie 'Mr. Nobody.'

node liri.js do-what-it-says

Using the fs Node package, LIRI will take the text inside of random.txt and then use it to call one of LIRI's commands.

do-what-it-says returns the result of a "random" result by reading the random.txt file and performing the command written in that file.
