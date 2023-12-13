## Java notes

# Do not overuse 


# Use checked exception for recoverables and run time exceptions for programming error


# Always declare checked exceptions individually, and document precisely the conditions under which each one is thrown using the Javadoc @throws tag. Don’t take the shortcut of declaring that a method throws some superclass of multiple 


 IllegalArgumentException
IllegalStateException :Object state is inappropriate for method invocati
Non-null parameter value is inappropriate
Parameter value is null where prohibited
IndexOutOfBoundsException
Index parameter value is out of range
 ConcurrentModificationException
Concurrent modification of an object has been d prohibited
 UnsupportedOperationException
Object does not support method




# To capture a failure, the detail message of an exception should contain the values of all parameters and fields that contributed to the exception. For example, the detail message of an IndexOutOfBoundsException should contain the lower bound, the upper bound, and the index value that failed to lie between the bounds. This information tells a lot about the failure. Any or all of the three values could be wrong. The index could be one less than the lower bound or equal to the upper bound (a “fencepost error”), 
