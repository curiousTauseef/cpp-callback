## Basic C++ Callback Example

A basic implementation of a C++ callback function.

### Some Background

Consider the case where there is a master C++ class which a member class. This member class has operations where certain events require callbacks to methods of the master class. Note that the case that required this investigation could not be solved using inheritance. In C++ 11 it is possible to use `std::function` and `std::bind` as seen in [this example](https://stackoverflow.com/questions/14189440/c-class-member-callback-simple-examples/14189561#14189561). This repo contains an alternate solution for all C++ versions.

Therefore the desired callback method needed to be passed to the member class in the form of a method pointer.

(convert these to MD links)
calling method through method pointers (and the reason "owner" is needed):
https://stackoverflow.com/questions/16276373/how-to-call-member-function-through-member-function-pointer
method pointer syntax:
https://stackoverflow.com/questions/36969471/c-how-to-make-function-pointer-to-class-method
function pointers in C:
https://stackoverflow.com/questions/840501/how-do-function-pointers-in-c-work