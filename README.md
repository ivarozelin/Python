

# Task 1: Resellers sales for August
- Description: A 3rd party company provides you every month with the data that contains the sales of your brand new bavarage named "Ginger Beer" in Bulgaria where you conduct a conmpetion among your re-sellers who will win the first prize of 50 000 USD.
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
 
    

  - Test 2:
  
    - input data:
    
      Lily-20-119.80
    
      Mikey-35-195.65
    
      Lily-30-179.70
    
      Alex-45-269.55
    
      Mikey-left

      data is provided

    - Expected output:

      
  

    
     



