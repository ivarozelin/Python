

# Task 1: Resellers sales for August
- Description: A 3rd party company provides you every month with the data that contains the sales of your brand new bavarage named "Ginger Beer" in Bulgaria where you conduct a conmpetion among your re-sellers who will win the first prize of 50 000 USD.
- Input data: You will be receiving lines in the following format: "{reseller}-{quantity}-{total amount}" until you receive
"data is provided".However, you might have lines that are invalid because the reseller left the competion. Such lines will be display in the format {reseller}-left".
- Specification: the data you receive is accumulative - this means the sales of the reseller each day includes the sales from previous day(s).
- Requirements:
  - If a reseller has two or more submissions for the same bavarage, save only the maximum quantity of it and then calculate the final price.
  - If the reseller left the compation but previously he sold some quantity, you shuld remove his name from the sales info but keep his data in the "Left" section.
- Desired data output: 
  - display only unique values
  - output format should be:
  ![image](https://github.com/ivarozelin/Python/assets/134283235/1bfbe8be-c629-4c61-9e21-4b347ae50522)

- Code document: see "Resellers sales for August" file in this repository.
- Test scenario:

    
     



