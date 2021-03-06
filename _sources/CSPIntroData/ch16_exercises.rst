..  Copyright (C)  Brad Miller, David Ranum, Jeffrey Elkner, Peter Wentworth, Allen B. Downey, Chris
    Meyers, and Dario Mitchell.  Permission is granted to copy, distribute
    and/or modify this document under the terms of the GNU Free Documentation
    License, Version 1.3 or any later version published by the Free Software
    Foundation; with Invariant Sections being Forward, Prefaces, and
    Contributor List, no Front-Cover Texts, and no Back-Cover Texts.  A copy of
    the license is included in the section entitled "GNU Free Documentation
    License".


.. setup for automatic question numbering.

.. 	qnum::
	:start: 1
	:prefix: 16-12-

Chapter 16 Exercises
---------------------

#.

    .. tabbed:: ch16ex1t

        .. tab:: Question

            Fix syntax 6 errors in the code below so that the code runs correctly. It should set ``combined`` to the concatenation of ``start`` and ``name``.  It should print the length of the combined string, print the combined string, and it should print the result of ``name * 3``.

            .. activecode:: ch16ex1q
                :nocodelens:

                name = 'Mark"
                start = "My name is '
                combined = start  name
                print(len(combined)
                print(combined)
                print name * 3

        .. tab:: Answer

            Change the first ``'`` to a ``"`` in line 1.  Change the ``"`` to a ``'`` in line 2.  Add a ``+`` after ``start`` in line 3.  Add a ``)`` at the end of line 4.  Add a ``(`` and ``)`` on line 6.

            .. activecode:: ch16ex1a
                :nocodelens:

                name = "Mark"
                start = 'My name is '
                combined = start + name
                print(len(combined))
                print(combined)
                print(name * 3)


        .. tab:: Discussion

            .. disqus::
                :shortname: cslearn4u
                :identifier: teachercsp_ch16ex1q

#.

    .. tabbed:: ch16ex2t

        .. tab:: Question

            Add code to line 1 so that the code below prints 14.

            .. activecode::  ch16ex2q
                :nocodelens:

                aString =
                bString = "bow"
                cString = (aString + bString) * 2
                print(len(cString))

        .. tab:: Answer

            ``aString`` can be any 4 character string

            .. activecode::  ch16ex2a
                :nocodelens:

                aString = "rain"
                bString = "bow"
                cString = (aString + bString) * 2
                print(len(cString))

        .. tab:: Discussion

            .. disqus::
                :shortname: teachercsp
                :identifier: teachercsp_ch16ex2q

#.

    .. tabbed:: ch16ex3t

        .. tab:: Question

           Fix the 5 syntax errors in the code below so that it runs.  It should print the length of ``myFirstList`` and print the result of ``myFirstList * 3``.  Then it should set ``mySecondList`` to the concatenation of ``myFirstList`` and a list containing ``321.4``.  Then it should print the value of ``mySecondList``.

           .. activecode::  ch16ex3q
                :nocodelens:

                myFirstList = [12,"ape"13]
                print(len(myFirstList)
                print(myfirstList * 3)
                mySecondList = myFirstList + [321.4
                print(mySecondList


        .. tab:: Answer

            Add a comma before the ``13`` on line 1.  Add a ``)`` at the end of line 2.  Change line 3 to ``myFirstList``.  Add a ``]`` at the end of line 4.  Add a ``)`` at the end of line 5.

            .. activecode::  ch16ex3a
                :nocodelens:

                myFirstList = [12,"ape",13]
                print(len(myFirstList))
                print(myFirstList * 3)
                mySecondList = myFirstList + [321.4]
                print(mySecondList)

        .. tab:: Discussion

            .. disqus::
                :shortname: teachercsp
                :identifier: teachercsp_ch16ex3q

#.

    .. tabbed:: ch16ex4t

        .. tab:: Question

            Fix the errors so that the procedure prints "My name is JohnJohn" and "19".

            .. activecode::  ch16ex4q
                :nocodelens:

                def nameProcedure(name):
                start = "My name is"
                combined = start * (name * 2)
                print(combined)
                print(len(combined)


                nameProcedure(John)

        .. tab:: Answer

            Add quotations around John on line 8. Add a space after "is" in line 2. In line 3, change the ``*`` after start to a ``+``. In line 5 add a ``)`` after combined. Indent lines 2 through 5.

            .. activecode::  ch16ex4a
                :nocodelens:

                def nameProcedure(name):
                    start = "My name is "
                    combined = start + (name * 2)
                    print(combined)
                    print(len(combined))


                nameProcedure("John")

        .. tab:: Discussion

            .. disqus::
                :shortname: teachercsp
                :identifier: teachercsp_ch16ex4q

#.

    .. tabbed:: ch16ex5t

        .. tab:: Question

           Fix 5 syntax errors in the code below so that it runs and prints the contents of ``items``.

           .. activecode::  ch16ex5q
                :nocodelens:

               def itemLister(items):
                   items[0] = "First item'
                   items[1] = items0]
                   items[2] = items[2] + 1
                   print items

                itemLister([2,4,6 8])

        .. tab:: Answer

            Add a ``,`` between 6 and 8 on line 7.  Change the ``'`` to a ``"`` on line 2.  Put a ``[`` before the 0 on line 3.  Add ``(`` before ``items`` and ``)`` after on line 5.

            .. activecode::  ch16ex5a
                :nocodelens:

                def itemLister(items):
                    items[0] = "First item"
                    items[1] = items[0]
                    items[2] = items[2] + 1
                    print(items)

                itemLister([2,4,6,8])

        .. tab:: Discussion

            .. disqus::
                :shortname: teachercsp
                :identifier: teachercsp_ch16ex5q

#.

    .. tabbed:: ch16ex6t

        .. tab:: Question

            Complete the code on lines 4 and 5 so that the function returns the average of a list of integers.

            .. activecode::  ch16ex6q
                :nocodelens:

                def gradeAverage(aList):
                    sum = 0
                    for num in aList:

                    average =
                    return average

                aList = [99, 100, 74, 63, 100, 100]
                print(gradeAverage(aList))

        .. tab:: Answer

            On line 4, add ``sum = sum + num`` and on line 5, add ``sum/ len(aList)``.

            .. activecode::  ch16ex6a
                :nocodelens:

                def gradeAverage(aList):
                    sum = 0
                    for num in aList:
                        sum = sum + num
                    average =  sum / len(aList)
                    return average

                aList = [99, 100, 74, 63, 100, 100]
                print(gradeAverage(aList))

        .. tab:: Discussion

            .. disqus::
                :shortname: teachercsp
                :identifier: teachercsp_ch16ex6q

#.

    .. tabbed:: ch16ex7t

        .. tab:: Question

           Fix the indention in the code below so that it runs correctly.  It should loop and add the current value of ``source`` to ``soFar`` each time through the loop.  It should also print the value of ``soFar`` each time through the loop.

           .. activecode::  ch16ex7q
                :nocodelens:

                source = ["This","is","a","list"]
                soFar = []
                for index in range(0,len(source)):
                soFar = [source[index]] + soFar
                print(soFar)

        .. tab:: Answer

            Indent lines 4 and 5 as shown below.

            .. activecode::  ch16ex7a
                :nocodelens:

                source = ["This","is","a","list"]
                soFar = []
                for index in range(0,len(source)):
                    soFar = [source[index]] + soFar
                    print(soFar)


        .. tab:: Discussion

            .. disqus::
                :shortname: cslearn4u
                :identifier: teachercsp_ch16ex7q

#.

    .. tabbed:: ch16ex8t

        .. tab:: Question

            Fix the code so that the code prints "['hihi', 0, 0, 4]" .

            .. activecode::  ch16ex8q
                :nocodelens:

                items = ["hi" 2, 3, 4]
                items[0] = items[0] * items0
                items(1) = items[2] - 3
                items[2] = items[1]
                print(items)

        .. tab:: Answer

            On line 1, add a ``,`` before "2". On line 2, it should be ``items[0]`` and a ``+`` instead of a ``*``. On line 3, it should be ``items[1]``.

            .. activecode::  ch16ex8a
                :nocodelens:

                items = ["hi", 2, 3, 4]
                items[0] = items[0] + items[0]
                items[1] = items[2] - 3
                items[2] = items[1]
                print(items)

        .. tab:: Discussion

            .. disqus::
                :shortname: teachercsp
                :identifier: teachercsp_ch16ex8q

#.

    .. tabbed:: ch16ex9t

        .. tab:: Question

           Fix 4 syntax errors in the code below.  After the code executes the list ``soFar`` should contain the reverse of the ``source`` list.

           .. activecode::  ch16ex9q
                :nocodelens:

                # setup the source list
                source = ["This","is" "a","list"]

                # Set the accumulator to the empty list
                soFar = [

                # Loop through all the items in the source list
                for index in range(0,len(source))

                    # Add the current item in the source and print the current items in soFar
                    soFar = [source[index]] + sofar
                    print(soFar)


        .. tab:: Answer

            Add a comma between ``is`` and ``a`` on line 2.  Add a ``]`` at the end of line 5.  Add a ``:`` at the end of line 8.  Change line 11 to ``soFar``.

            .. activecode::  ch16ex9a
                :nocodelens:

                # setup the source list
                source = ["This","is","a","list"]

                # Set the accumulator to the empty list
                soFar = []

                # Loop through all the items in the source list
                for index in range(0,len(source)):

                    # Add the current item in the source and print the current items in soFar
                    soFar = [source[index]] + soFar
                    print(soFar)


        .. tab:: Discussion

            .. disqus::
                :shortname: teachercsp
                :identifier: teachercsp_ch16ex9q

#.

    .. tabbed:: ch16ex10t

        .. tab:: Question

            The code below currently prints the reverse of a list. Change it so that it prints a mirrored version of the list. It should print "['list', 'a', 'is', 'This', 'This', 'is', 'a', 'list']".

            .. activecode::  ch16ex10q
                :nocodelens:

                # setup the source list
                source = ["This","is","a","list"]

                # Set the accumulator to the empty list
                soFar = []

                # Loop through all the items in the source list
                for index in range(0,len(source)):

                    # Add a list with the current item from source to soFar
                    soFar =  [source[index]] + soFar
                print(soFar)

        .. tab:: Answer

            In the for loop make ``soFar`` equal to ``[source[index]] + soFar + [source[index]]``.

            .. activecode::  ch16ex10a
                :nocodelens:

                # setup the source list
                source = ["This","is","a","list"]

                # Set the accumulator to the empty list
                soFar = []

                # Loop through all the items in the source list
                for index in range(0,len(source)):

                    # Add the lists with the current item from source to soFar
                    soFar =  [source[index]] + soFar + [source[index]]
                print(soFar)


        .. tab:: Discussion

            .. disqus::
                :shortname: teachercsp
                :identifier: teachercsp_ch16ex10q

#.

    .. tabbed:: ch16ex11t

        .. tab:: Question

           Change the following code into a function.  It should take the list and return a list of the values at the even indicies.

           .. activecode::  ch16ex11q
                :nocodelens:

                numbers = [0,1,2,3,4,5,6,7,8,9,10]
                evenList = []
                for index in range(0,len(numbers),2):
                    evenList = evenList + [numbers[index]]
                print(evenList)




        .. tab:: Answer

            Define a function that takes a list and then call the function and pass in the list.  Print the result.

            .. activecode::  ch16ex11a
                :nocodelens:

                def getEvenIndicesList(numbers):
                    evenList = []
                    for index in range(0,len(numbers),2):
                        evenList = evenList + [numbers[index]]
                    return(evenList)

                print(getEvenIndicesList([0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10]))

        .. tab:: Discussion

            .. disqus::
                :shortname: teachercsp
                :identifier: teachercsp_ch16ex11q

#.

    .. tabbed:: ch16ex12t

        .. tab:: Question

            The following code creates and prints a list of even numbers. Change it and add to it so that it creates a list of all multiples of 5 from 0 to 50, inclusive.

            .. activecode::  ch16ex12q
                :nocodelens:

                # initialize the variables
                numbers = [0,1,2,3,4,5,6,7,8,9,10]
                evens = []

                # loop though every other index
                for index in range(0,len(numbers),2):

                    # add the lists
                    evens = evens + [numbers[index]]

                # print the result
                print(evens)

        .. tab:: Answer

            Change  ``numbers`` to equal ``range(1,51,5)`` and the range in the for loop to (0,len(numbers)).

            .. activecode::  ch16ex12a
                :nocodelens:

                # initialize the variables
                numbers = range(1,51,5)
                fives = []

                # loop though every index
                for index in range(0,len(numbers)):

                    # add the lists
                    fives = fives + [numbers[index]]

                # print the result
                print(fives)

        .. tab:: Discussion

            .. disqus::
                :shortname: teachercsp
                :identifier: teachercsp_ch16ex12q

#.

    .. tabbed:: ch16ex13t

        .. tab:: Question

           Change the following into a procedure. It prints a countdown from 5 to 0.  Have it take the starting number for the countdown as a parameter.  Print each value till it gets to 0.

           .. activecode::  ch16ex13q
                :nocodelens:

                for index in range(5, -1, -1):
                    print(index)




        .. tab:: Answer

            Define the procedure and call it.  Be sure to pass the number to start the countdown at.

            .. activecode::  ch16ex13a
                :nocodelens

                def countdown(start):
                    for index in range(start, -1, -1):
                        print(index)

                countdown(10)


        .. tab:: Discussion

            .. disqus::
                :shortname: teachercsp
                :identifier: teachercsp_ch16ex13q

#.

    .. tabbed:: ch16ex14t

        .. tab:: Question

            Fix the errors so that the code individually adds each item from ``source`` to ``newList``. Make the range decrement, so it starts from the end, but keep ``newList`` in the same order as ``source``.


            .. activecode::  ch16ex14q
                :nocodelens:

                # initialize the variables
                source = ["This","is","a","list"]
                newList = []

                # loop from the last index to the first (0)
                for index in range(len(source), 1, -1):

                # append the lists
                newList = newList + [source[index]]

                # print the current value of the list
                print(newList)

        .. tab:: Answer

            On line 6, the range should be ``(len(source) - 1, -1, -1)``. Indent line 9 and switch the order the items are added.

            .. activecode::  ch16ex14a
                :nocodelens:

                # initialize the variables
                source = ["This","is","a","list"]
                newList = []

                # loop from the last index to the first (0)
                for index in range(len(source) - 1, -1, -1):

                    # append the lists
                    newList = [source[index]] + newList

                # print the current value of the list
                print(newList)

        .. tab:: Discussion

            .. disqus::
                :shortname: teachercsp
                :identifier: teachercsp_ch16ex14q

#.

    .. tabbed:: ch16ex15t

        .. tab:: Question

           Write a function that returns the values at the odd indices in a list.  The function should take the number list as a parameter.  If it is passed [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10] for example, it should return [1, 3, 5, 7, 9].

           .. activecode::  ch16ex15q
                :nocodelens:


        .. tab:: Answer

            See the function below.  Be sure to create the function and call it and print the result.

            .. activecode::  ch16ex15a
                :nocodelens:

                def getOddIndicesList(numbers):
                    evenList = []
                    for index in range(1,len(numbers),2):
                        evenList = evenList + [numbers[index]]
                    return(evenList)

                print(getOddIndicesList([0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10]))

        .. tab:: Discussion

            .. disqus::
                :shortname: teachercsp
                :identifier: teachercsp_ch16ex15q

#.

    .. tabbed:: ch16ex16t

        .. tab:: Question

            Write a function that takes a list of numbers as a parameter and adds 5 to each number and returns the list.

            .. activecode::  ch16ex16q
                :nocodelens:


        .. tab:: Answer

            You need to know the index of each item in the list so use the range function in the for loop.

            .. activecode::  ch16ex16a
                :nocodelens:

                def listAdder(aList):
                    for x in range(len(aList)):
                        aList[x] = aList[x] + 5
                    return aList
                nums = [1,2,3]
                print(listAdder(nums))

        .. tab:: Discussion

            .. disqus::
                :shortname: teachercsp
                :identifier: teachercsp_ch16ex16q

#.

    .. tabbed:: ch16ex17t

        .. tab:: Question

           Write a function that takes a list of numbers and returns the sum of the positive numbers in the list.

           .. activecode::  ch16ex17q
                :nocodelens:

        .. tab:: Answer

            Define the function as shown below.  Be sure to accumulate and return the sum.  Call the function and print the result.

            .. activecode::  ch16ex17a
                :nocodelens:

                def sumPos(theList):
                    sum = 0
                    for item in theList:
                        if item >= 0:
                            sum = sum + item
                    return sum

                print(sumPos([-3, 2, -8, 5, -20, -33, 15]))


        .. tab:: Discussion

            .. disqus::
                :shortname: teachercsp
                :identifier: teachercsp_ch16ex17q

#.

    .. tabbed:: ch16ex18t

        .. tab:: Question

            Write a function that takes in a list of numbers as a parameter. The function should calculate the sum of all the positive numbers in the list, the absolute value of the sum of the negative numbers, and return the average of the two sums.

            .. activecode::  ch16ex18q
                :nocodelens:

        .. tab:: Answer

            Define the function as shown below.

            .. activecode::  ch16ex18a
                :nocodelens:

                def aFunction(aList):
                    posSum = 0
                    negSum = 0
                    for x in aList:
                        if x >= 0:
                            posSum = posSum + x
                        else:
                            negSum = negSum + x
                    avg = (posSum + (negSum * -1))/2
                    return avg

                nums = [-3,-1,2,4]
                print(aFunction(nums))

        .. tab:: Discussion

            .. disqus::
                :shortname: teachercsp
                :identifier: teachercsp_ch16ex18q

#.

    .. tabbed:: ch16ex19t

        .. tab:: Question

           Write a function to return the reverse of a list, but with only every other item from the original list starting at the end of the list.  So, if it is passed the list [0,1,2,3,4,5] for example, it should return the list [5, 3, 1].

           .. activecode::  ch16ex19q
               :nocodelens:

        .. tab:: Answer

            Define the function as shown below.

            .. activecode::  ch16ex19a
                :nocodelens:

                def reverseEveryOther(theList):
                    newList = []
                    for index in range(len(theList) - 1, -1, -2):
                        newList = newList + [theList[index]]
                    return newList


                print(reverseEveryOther([0,1,2,3,4,5]))


        .. tab:: Discussion

            .. disqus::
                :shortname: teachercsp
                :identifier: teachercsp_ch16ex19q

#.

    .. tabbed:: ch16ex20t

        .. tab:: Question

            Write a procedure that takes an int as a parameter. The procedure should add every other odd number from 1 to the int parameter (inclusive) into a new list. The procedure should print the new list and the sum of the new list.

            .. activecode::  ch16ex20q
                :nocodelens:

        .. tab:: Answer

            Define the procedure as below.

            .. activecode::  ch16ex20a
                :nocodelens:

                def aProcedure(num):
                    newList = []
                    sum = 0
                    for i in range(1, num + 1, 4):
                        newList = newList + [i]
                        sum = sum + i
                    print(newList)
                    print(sum)
                aProcedure(20)

        .. tab:: Discussion

            .. disqus::
                :shortname: teachercsp
                :identifier: teachercsp_ch16ex20q
