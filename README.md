import random 
import time 
import os
import sys

def delete_last_line():
    "Use this function to delete the last line in the STDOUT"

    #cursor up one line
    sys.stdout.write('\x1b[1A')

    #delete last line
    sys.stdout.write('\x1b[2K')

outPut = []
def changer():
    outPut.append(input("add a number: "))
    delete_last_line()
    print(outPut)
    time.sleep(2)
    delete_last_line()
while True:
    time.sleep(.5)    
    changer()    
