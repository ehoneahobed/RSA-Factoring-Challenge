#!/usr/bin/python3
"""Module that factorize as many numbers as possible
 into a product of two smaller numbers."""
from sys import argv


def factorize(value):
    """"print a simple descomposition of an integer > 1"""
    i = 2

    if value < 2:
        return
    print()
    print(value, "<- value-bef")
    while value % i:
        i += 1
    print("{:.0f}={:.0f}*{:.0f}".format(value, value / i, i))
    print(value, "<- value-aft")
    print()

if len(argv) != 2:
    exit()

try:
    with open(argv[1]) as file:
        line = file.readline()

        while line != "":
            value = int(line.split('\n')[0])
            factorize(value)
            line = file.readline()
except:
    pass
