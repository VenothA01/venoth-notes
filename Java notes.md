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

NOTES ON 12 FACTOR APP

https://medium.com/@tech_18484/introduction-701b7a8f4730


![Build img](https://github.com/VenothA01/venoth-notes/blob/master/MethodToBuilAsSaas.png)

Codebase
:-One codebase is tracked in version control.
:-Multiple deployments share the same codebase.

Dependencies
:-Explicitly declare and isolate dependencies.
:-Avoid relying on system-wide packages.

Config
:-Store configuration in the environment.
:-Separate configuration from code

Backing Services
:-Treat backing services (databases, caches) as attached resources.
:-Access them via environment variables.

Build, Release, Run
:-Strictly separate build, release, and run stages.
:-Keep builds and releases immutable

Processes
:-Execute the app as stateless processes.
:-Store shared state in databases or external services

Port Binding
:-Export services via port binding.
:-Keep the app self-contained.

Concurrency
:-Scale out via the process model.
:-Enable horizontal scaling.

Disposability
:-Maximize robustness with fast startup and graceful shutdown.
:-Aim for quick startup and graceful handling of process failures.

Dev/Prod Parity
:-Keep development, staging, and production environments as similar as possible.
:-Minimize differences to reduce bugs.

Logs
:-Treat logs as event streams.
:-Stream logs to a centralized location for analysis.

Admin Processes
:-Run admin/management tasks as one-off processes.
:-Avoid mixing them with the main application code


