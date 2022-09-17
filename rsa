#!/usr/bin/python3
"""
Factorize as many numbers as possible into a product of two smaller numbers.
    Usage: factors <file>
        where <file> is a file containing natural numbers to factor.
        One number per line
        You can assume that all lines will be valid natural numbers\
                greater than 1
        You can assume that there will be no empy line, and no space\
                before and after the valid number
        The file will always end with a new line
    Output format: n=p*q
        one factorization per line
        p and q don’t have to be prime numbers
        See example
    You can work on the numbers of the file in the order of your choice
    Your program should run without any dependency: You will not be ablei\
            to install anything on the machine we will run your program on
    Time limit: Your program will be killed after 5 seconds\
            if it hasn’t finish
    Push all your scripts, source code, etc… to your repository
"""
# library to get arguments
import sys


# fn unpack number factorial
def fc():
    """
    function fc to search file to convert number and format n=p*q
    """
    try:
        revfile = sys.argv[1]
        with open(revfile) as f:
            for revnumber in f:
                revnumber = int(revnumber)
                if revnumber % 2 == 0:
                        print("{}={}*{}".format(revnumber, revnumber // 2, 2))
                        continue
                i = 3
                while i < revnumber // 2:
                    if revnumber % i == 0:
                        print("{}={}*{}".format(revnumber, revnumber // i, i))
                        break
                    i = i + 2
                if i == (revnumber // 2) + 1:
                    print("{}={}*{}".format(revnumber, revnumber, 1))
    except (IndexError):
        pass


# autostart
fc()
