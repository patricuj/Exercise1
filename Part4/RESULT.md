i = 0

def incrementingFunction():

    global i
    
    i += 1000000

def decrementingFunction():

    global i
    
    i -= 1000000

    def main():
        print(i)

        incrementing = Thread(target = incrementingFunction, args = (),)
        decrementing = Thread(target = decrementingFunction, args = (),)

        incrementing.join()
        decrementing.join()

        print("The magic number is %d" % (i))


main()
