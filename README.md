

# Task 1: Resellers sales for August
- Description: A 3rd party company provides you every month with the data that contains the sales of your brand new bavarage named "Ginger Beer" in Bulgaria.
- Input data: You will be receiving lines in the following format: "{reseller}-{quantity}-{bottle price}" until you receive
"data is provided".However, you might have lines that are invalid because the reseller left the competion. Such lines will be display in the format {reseller}-left".
- Specification: the data you receive is accumulative - this means the sales of the reseller each day includes the sales from previous day(s).
- Requirements:
  - If a re-seller has two or more submissions for the same bavarage, save only the maximum quantity of it and then calculate the final price.
  - If the re-seller left the compation but previously he sold some quantity, you shuld remove his name from the sales info but keep his data in the "Left" section.
  - if no re-seller left the competition, don`t display the "Left" print.
- Desired data output: 
  - display the resellers only ones
  - output format should be:
   
    ![image](https://github.com/ivarozelin/Python/assets/134283235/57512d21-17f7-4ff5-a8be-62082940aa5b)

- Code document: see "Resellers sales for August" file in this repository.
- Test scenario:
  
  - Test 1:

    - Input data:
    
      Lily-20-119.80
    
      Mikey-35-195.65
    
      Lily-30-179.70
    
      Alex-45-269.55
    
      data is provided

    - Expected output:
      
      Sales in August:
      
      Lily | 179.7
      
      Mikey | 195.65
      
      Alex | 269.55 

  - Test 2:
  
    - input data:
    
      Lily-20-119.80
    
      Mikey-35-195.65
    
      Lily-30-179.70
    
      Alex-45-269.55
    
      Mikey-left

      data is provided

    - Expected output:

      Sales in August:

      Lily-30-179.70
    
      Alex-45-269.55

      Left:

      Mikey-35-195.65
      

# Task 2: Secret chat

- Desription: On the first line of the input, you will receive the concealed message. After that, until the "Reveal" command is
given, you will receive strings with instructions for different operations that need to be performed upon the
concealed message to interpret it and reveal its actual content.

  There are several types of instructions, split by ":|:"

- "InsertSpace:|:{index}":

  - Inserts a single space at the given index. The given index will always be valid.
    
- "Reverse:|:{substring}":

  - If the message contains the given substring, cut it out, reverse it and add it at the end of the
message.

  - If not, print "error".
    
  - This operation should replace only the first occurrence of the given substring if there are two or
more occurrences.

- "ChangeAll:|:{substring}:|:{replacement}":
  
    - Changes all occurrences of the given substring with the replacement text.

- Input: 

  - On the first line, you will receive a string with a message.
  - 
  - On the following lines, you will be receiving commands, split by ":|:".

- Desired output:

  - After each set of instructions, print the resulting string.
    
  -  After the "Reveal" command is received, print this message: "You have a new text message: {message}"
 
  -  Test:
      - inout data:
 
        heVVodar!gniV
  
        ChangeAll:|:V:|:l
  
        Reverse:|:!gnil
  
        InsertSpace:|:5
  
        Reveal

     - output data:

       hellodar!gnil
       
       hellodarling!
       
       hello darling!
       
        You have a new text message: hello darling!
  

# Task 3 - Vehicle
- Description: create a class Vehicle.
  
- Requirements:
  
    The class should have the following methods:
  
      - buy(money: int, owner: str)
  
        - If the person has enough money and the vehicle has no owner, returns: "Successfully bought a {type}. Change: {change}" and sets the owner to the given one
  
        - If the money is not enough, return: "Sorry, not enough money"
  
        - If the car already has an owner, return: "Car already sold"
  
    - sell()
      
        - If the car has an owner, set it to None again.
          
        - Otherwise, return: "Vehicle has no owner"
          
    - __repr__()
      
      - If the vehicle has an owner, returns: "{model} {type} is owned by: {owner}".
        
      - Otherwise, return: "{model} {type} is on sale: {price}"
     
  - Test:
    
    - Input data:

      vehicle_type = "car"
      
      model = "BMW"
      
      price = 30000
      
      vehicle = Vehicle(vehicle_type,model, price)
      
      print(vehicle.buy(15000, "Peter"))
      
      print(vehicle.buy(35000, "George"))
      
      print(vehicle)
      
      vehicle.sell()
      
      print(vehicle)

  - Expected output:

    Sorry, not enough money
    
    Successfully bought a car. Change: 5000.00
    
    BMW car is owned by: George
    
    BMW car is on sale: 30000

      
  

    
     



