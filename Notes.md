class Person
  def initialize(name)
    @name = name
  end

  def name
    @name
  end
end

kanye = Person.new("Kanye")
kanye.name #=> "Kanye"
 

 # name is considered a "getter" or a "reader"
 # in order to make it #name writable (being able to change,delet,etc.)
 # we need to define the "setter" or a "writer" method


 class Person

  def initialize(name)
    @name = name
  end

  def name
    @name
  end

  def name=(new_name)
    @name = new_name
  end

end 


# A setter method is defined with an =, equals sign, appended to the name of the method. The = is followed by the (argument_name)

Note: The syntax highlighting may make it look like the = sign in name= is separate from the name of the definition, but it is not. The = is a necessary piece. Adding it in allows us to write kanye.name = "Yeezy" but this is a bit of syntatic sugar. Writing kanye.name=("Yeezy") is also a valid way to use this setter method.

# Now to call a Setter Method
To call a setter method, you use the . notation (dot notation) to call the method and set it equal to a new value.

kanye = Person.new("Kanye")

kanye.name
  => "Kanye"

kanye.name = "Yeezy"
kanye.name
  => "Yeezy" 


# Let's break it down. We:

Instantiate a Person instance and name him "Kanye".
Call our getter method, #name to return his name, "Kanye"
Call our setter method #name= to change his name to "Yeezy"
Call our getter method again and see that kanye's name is now "Yeezy".


# You can also call a setter method like this:

kanye.name=("Yeezy") 