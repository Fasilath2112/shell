# Automated Readability Index (ARI)

*The Automated Readability Index (ARI) is a test used to measure how easy or difficult a text is to read. The ARI formula gives a number that estimates the grade level a person needs to be at to understand the text.*

### The formula for ARI is:

**ARI = 4.71 × (characters / words) + 0.5 × (words / sentences) − 21.43**

## Objective:

*This project aims to create a bash script for calculating the ARI score of a text file. The script will take a file as input, analyze its content, apply the ARI formula, and output the readability score.*

## Steps for creating the ARI Program:

1. **Reading**: The script will read the content of the file provided as an argument.

2. **Text elements calculation**: Utilize bash commands to count the characters, words, and sentences in the text.

3. **ARI Calculation**: Apply the ARI formula using the calculated values.

4. **Displaying the Result**: Output the computed ARI score.

5. **Finalizing the Script**: Combine all the components to create the final bash script.

## Challenges Faced:

<span style="color:red">**Handling Floating-Point Numbers**</span>: Bash does not support floating-point arithmetic. It only supports integer arithmetic. So we need to use external tools.

<span style="color:red">**Text Counting**</span>: Accurately analyzing text to count characters, words, and sentences is challenging. This requires careful handling of whitespace, punctuation, and special characters.

<span style="color:red">**Precision Issues**</span>: When performing arithmetic operations like division, precision issues can arise due to the limited precision of floating-point arithmetic.

## Solutions Implemented:

<span style="color:green">**'bc'**</span> is used to handle floating-point numbers when applying the ARI equation.

<span style="color:green">**'grep'**</span> with regular expressions was used to count sentences more precisely.

The <span style="color:green">**`printf`**</span> command with the <span style="color:green">**`%.2f`**</span> format specifier was used to display the ARI score with two decimal places, providing a clear and precise output.

## Conclusion:

*Using the above steps, the script reads the text file and determines the count of characters, words, and sentences. It checks conditions, applies the ARI equation, and gives the output with the grade level. Thus, it successfully calculates the Automated Readability Index of a given text file. This script is helpful to understand the readability level of text files ranging from kindergarten to college.*
