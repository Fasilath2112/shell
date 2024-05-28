## Automated Readability Index (ARI)

     The Automated Readability Index (ARI) is a test used to measure how easy or difficult a text is to read. The ARI formula gives a number that estimates the grade level a person needs to be at to understand the text.

The formula for ARI is:

     ARI=4.71×(characterswords)+0.5×(wordssentences)−21.43ARI=4.71×(wordscharacters​)+0.5×(sentenceswords​)−21.43

### Objective:

    This project aims to create a bash script for calculating the ARI score of a text file. The script will take a file as input, analyze its content, apply the ARI formula, and output the readability score.

### Steps for creating the ARI Program:

    File Reading: The script will read the content of the file provided as an argument.

    Text elements calculation: Utilize bash commands to count the characters, words, and sentences in the text.

    ARI Calculation: Apply the ARI formula using the calculated values.

    Displaying the Result: Output the computed ARI score.

    Finalizing the Script: Combine all the components to create the final bash script.
    
### Challenges Faced:

    Handling Floating-Point Numbers: Bash does not support floating-point arithmetic. It only supports integer arithmetic. So we need to use external tools.

    Text Counting: Accurately analyzing text to count characters, words, and sentences is challenging. This requires careful handling of whitespace, punctuation, and special characters.

    Precision Issues: When performing arithmetic operations like division, precision issues can arise due to the limited precision of floating-point arithmetic.


### Solutions Implemented:

    Handling Floating-Point Numbers: 'bc' is used to handle floating point numbers when applying ARI equation.

    Text Counting: 'grep' with regular expressions was used to count sentences more precisely.

    Precision Issues: The `printf` command with the `%.2f` format specifier was used to display ARI score with two decimal places, providing a clear and precise output. 


### Conclusion:
    
    Using the above steps the script reads the text file and determine the count of characters, words, and sentences. Checks conditions, applied ARI equation and give the output with grade level. Thus successfully calculates the Automated Readability Index of a given text file. This script is helpful to understand the readability level of text files ranging from kindergarden to college. 




    
    
    
    


