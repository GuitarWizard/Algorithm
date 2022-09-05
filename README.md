# Algorithm

# Algorithms
# Write a script which prints all the permutations of a string in alphabetical order. We consider that
# digits < upper case letters < lower case letters. The sorting should be performed in ascending
# order.
# Your program should accept a file as its first argument. The file contains input strings, one per
# line. Print to stdout the distinct permutations of the string separated by comma, in alphabetical
# order.

# Contents of sample input file:
# hat abc Zu6 T AA

# Expected output for the input above:
# aht,ath,hat,hta,tah,tha
# abc,acb,bac,bca,cab,cba
# 6Zu,6uZ,Z6u,Zu6,u6Z,uZ6
# T
# AA


The program reads a .csv file containing all the strings that are to be permutated per the description above.

The functions within the program are executed in the following order per the execution section starting on line 97:

read_file():
    """Reads an input file in the program's home directory. Input file must be a .csv file
    Program returns a list of stings"""

compile_results(input_list):
    """Takes the input list of strings, and individually runs them through the permutate function
    to get all possible combinations of rearranged characters. Returns the combinations into a new list named
    compiled_text_list. Returns the compiled_text_list.

        inputs| input_list - a list of words to be scrambled"""
        
        
Executed via for loop in the compile_results function:
permutate(list_item):
    """Takes a string and creates all possible permutations of the individual characters rearranged. Additionally,
    it sorts the generated permuations into alphabetical order. The function also eliminates duplicate permutations.
    Example: an entry of AA or BB will only return AA or BB, not AA, AA, and BB, BB

        inputs| list_item: the item desired to be permutated"""


output_results(final_composition):
    """Takes the list of finalized collections of permutations and exports them by stdout, one collection per line.
    This function does not return a value, only outputs data via stdout.
        inputs| final_composition - a list of lists of alphabetically sorted permutations. """
