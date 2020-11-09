## Naming variables
 - As you know, every variable has a name that uniquely identifies it among other variables. Giving a good name to 
 a variable may not be as simple as it seems. Experienced programmers are careful when naming their variables to ensure that their programs are easy to
 understand. It is important because programmers spend a lot of time reading and understanding code written by other programmers. If variables have bad names, even your own code 
 will seem unclear to you in a few months.
 ## Code style convention
  PEP 8 provides some rules for variable names to increase code readability.
 - #### Use lowercase and underscores to split words. Even if it's an abbreviation
     
     
       http_response  # yes!
       httpresponse   # no
       myVariable     # no, that's from Java
 However, if you want to define a constant, it's common to write its name in all capital letters and, again, separate words with underscores. Normally, constants are stored in special files called modules.
     
     
      SPEED_OF_LIGHT = 299792458
    
 - #### Avoid names of one letter that could be easily mixed up with numbers like 'l' (lowercase letter el), 'O' (uppercase letter oh), or 'I' (uppercase letter eye).
        
       l = 1    # no
       O = 100  # no, if you use this variable name further in your code it would look like zero
     
 - #### Although you can use any Unicode symbols, the code style convention recommends limiting variable names with ASCII characters.
       
         # Using Cyrillic instead of Latin can cause an evening of useless headache
         # These are different variables!
         copy = "I'm written in Latin alphabet"        # yes!
         сору = "And I'm written in Cyrillic!"  # no
 - #### If the most suitable variable name is some Python keyword, add an underscore to the end of it.
          
         class_ = type(var)  # yes!
         klass = type(var)   # no
