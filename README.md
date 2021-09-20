# error_handling

https://docs.python.org/2/library/exceptions.html#exception-hierarchy
```
BaseException
 +-- SystemExit
 +-- KeyboardInterrupt
 +-- GeneratorExit
 +-- Exception
      +-- StopIteration
      +-- StandardError
      |    +-- BufferError
      |    +-- ArithmeticError
      |    |    +-- FloatingPointError
      |    |    +-- OverflowError
      |    |    +-- ZeroDivisionError
      |    +-- AssertionError
      |    +-- AttributeError
      |    +-- EnvironmentError
      |    |    +-- IOError
      |    |    +-- OSError
      |    |         +-- WindowsError (Windows)
      |    |         +-- VMSError (VMS)
      |    +-- EOFError
      |    +-- ImportError
      |    +-- LookupError
      |    |    +-- IndexError
      |    |    +-- KeyError
      |    +-- MemoryError
      |    +-- NameError
      |    |    +-- UnboundLocalError
      |    +-- ReferenceError
      |    +-- RuntimeError
      |    |    +-- NotImplementedError
      |    +-- SyntaxError
      |    |    +-- IndentationError
      |    |         +-- TabError
      |    +-- SystemError
      |    +-- TypeError
      |    +-- ValueError
      |         +-- UnicodeError
      |              +-- UnicodeDecodeError
      |              +-- UnicodeEncodeError
      |              +-- UnicodeTranslateError
      +-- Warning
           +-- DeprecationWarning
           +-- PendingDeprecationWarning
           +-- RuntimeWarning
           +-- SyntaxWarning
           +-- UserWarning
           +-- FutureWarning
	   +-- ImportWarning
	   +-- UnicodeWarning
	   +-- BytesWarning
	   
```
     
https://www.learnpython.dev/03-intermediate-python/40-exceptions/99-exercise/
https://werkzeug.palletsprojects.com/en/2.0.x/exceptions/
     
class UnAcceptedValueError(Exception):   
    def __init__(self, data):    
        self.data = data
    def __str__(self):
        return repr(self.data)

Total_Marks = int(input("Enter Total Marks Scored: "))
try:
    Num_of_Sections = int(input("Enter Num of Sections: "))
    if(Num_of_Sections < 1):
        raise UnAcceptedValueError("Number of Sections can't be less than 1")
except UnAcceptedValueError as e:
    print ("Received error:", e.data)
    
https://www.geeksforgeeks.org/built-exceptions-python/
https://www.geeksforgeeks.org/user-defined-exceptions-python-examples/
https://docs.python.org/3/tutorial/errors.html?fbclid=IwAR2qr-ZvGT4H8qhK2iEGhOQxxBbMofwK29XpFdLUVGDE4vDdXnDrUk6miFI

https://python-forum.io/thread-18065.html 
https://recalll.co/?q=python%20-%20urllib2%20HTTP%20error%20429%20-%20Stack%20Overflow&type=code
https://www.youtube.com/watch?v=aBexJgZ6GjI
https://stackoverflow.com/questions/53611767/using-super-and-init-in-custom-exceptions/53611859
https://stackoverflow.com/questions/2901000/the-correct-way-to-define-an-exception-in-python-without-pylint-complaining

     
     
     
     
