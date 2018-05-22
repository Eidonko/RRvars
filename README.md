# RRvars
A reactive layer for the C programming language

I propose an approach and simple tool for the expression of tasks such as cross-layer optimization strategies or sensors-related applications. The approach is based on what I call as “reflective and refractive variables” -- variables that are associated with external sensors or actuators. A reflective variable is a volatile variable (that is, a variable that can be concurrently modified by threads). A library of threads is made available, each of which interfaces a set of sensors and continuously updates the value of a corresponding set of sensors. One such thread is “cpu”, which exports the current level of usage of the local CPU as an integer between 0 and 100. This integer is reflected into the integer reflective variable with the same name. Callback functions can be defined, which automatically call a user defined function when an expression on reflective variables is satisfied.
