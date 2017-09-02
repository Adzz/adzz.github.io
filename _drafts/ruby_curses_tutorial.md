dispel gem?


Exploring the terminal with ruby:

`control - v` and then a key press will print the escape code for the key.
For example, is not good enough to just simply type puts "^[[31;49m", you have to do ctrl - v esc in the place of "^["

can iterate over colors to see what they do:


39 - default foregorund
49m - default background color

puts "^[[31;49mfoooo" will leave the terminal in whatever

state we left it
adding to the end:

puts "^[[31;49mfoooo^[[39:49m"

we can reset after we done.


we can also write a loop to see what the numbers do:

10.upto(50) do |x|
  puts "^[[#{x};49mfoooo^[[39:49m"
end


OTHER BLOGS

Cat theory talk into series of blog posts
Back to front end posts on blog
Exploring the terminal with ruby

Learning elixir

========= FUN ONE =========================
The difference between code telling us what it does
and telling us how it does it. Sometimes we want to know
one and sometimes the other. Explore with an example
