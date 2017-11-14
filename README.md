# microservice_debugger

When using microservices, it can be hard to debug problems holistically. If a single service fails, it's often obvious where that service failed and why, but it can be hard to debug problems in microservices that occur between microservices. If a platform has thousands of users, finding the issue that one user is experiencing can be like finding a needle in a haystack. This program intends to fix this.


# Goals
 * support the identification of common user-defined problems and execution of solutions. 
 * when a problem cannot be solved automatically, make it easy for someone to come in and quckly determine the cause
 * be transport and language independent. To start with, I'd like to support using Go, but this will be designed in such a way that it's easy to extend with another language. This should be designed to be platform agnostic, whether communication is over kafka, REST, or something else, this platform should be easy to extend with additional transports.
 * This should be production ready.
