# ECE444-F2023-Lab5"

What are the pros and cons of TDD?

Test Driven Development (TDD) is a software development methodology that puts an emphasis on testing throughout the software development lifecycle, rather than backloading it at the end of development. It encourages develompent of tests in parallel with (or prior to) implementation of code, which is continuously updated and evaluated. 

One advantage of TDD is that it promotes early detection of defects, reducing the eventual cost of repairing it. Defects caught early can be repaired, in general, at lesser cost than defects caught later. For example, defects generated at the requirements stage incur exponentially greater costs to repair over time, as discussed in lecture.

Another advantage is that, since design thinking is oriented towards testing before implementation, developers can focus on exactly what the software artifact should do and how it should behave before implementing it. Forced frontloading of detailed design thinking accelerates later implementation, as the precise details of expected input and output will be well known prior to writing any code. This focus promotes higher quality code.

One disadvantage is that TDD significantly slows the pace of development - mandating that unit tests should be written before implementation adds friction to the development process, and delaying implementation doesn't always lead to better results (as unexpected ideas or consequencse always arise).

Another disadvantage is the requirement of additional software infrastructure and compute to run tests. Overtesting can happen, which strains resources and incurs costs. For example, a team relying on TDD may run full system integration tests every time a commit is checked in, so any minor changes may require hours of compute to verify, potentially rented at cost from cloud service providers like AWS. 