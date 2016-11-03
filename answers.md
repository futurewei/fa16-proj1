# Q0: Why is this error being thrown?
since we dont have pokemon model yet.

# Q1: How are the random Pokemon appearing? What is the common factor between all the possible Pokemon that appear? *
it appears as text on the screen. They're generated after we type rake db:seed. 

# Question 2a: What does the following line do "<%= button_to "Throw a Pokeball!", capture_path(id: @pokemon), :class => "button medium", :method => :patch %>"? Be specific about what "capture_path(id: @pokemon)" is doing. If you're having trouble, look at the Help section in the README.

this will create something like /capture/1 if @pokemon passed in is 1. Passing a hash into the capture_path function basically passes in some params to generate the route.

# Question 3: What would you name your own Pokemon?
I named a lot pokemons, but the one I like the most is pikachu

# Question 4: What did you pass into the redirect_to? If it is a path, what did that path need? If it is not a path, why is it okay not to have a path here?
I passed something like redirect_to trainer_path(@pokemon.trainer). the paramater is something to be appended after the trainer_path. And I also redirect_to '/' which goes to the root.

# Question 5: Explain how putting this line "flash[:error] = @pokemon.errors.full_messages.to_sentence" shows error messages on your form.
I guess why it's named as flash is because it very quickly displaying the error message. so if users enter a duplicate name, it will show error.

# Give us feedback on the project and decal below!
so far very good. (I hope to learn how to quickly build up our website using bootstrap templates )

# Extra credit: Link your Heroku deployed app
