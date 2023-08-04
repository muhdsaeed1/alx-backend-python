Unit Test vs. Integration Test: Tell Them Apart and Use Both

Many people, upon hearing “automated testing,” automatically think of unit tests. That’s understandable; after all, unit testing is one of the most well-known types of automated tests. However, it’s far from being the only one. We have UI testing, end-to-end testing, load testing, and that’s just to name a few.

Defining Unit Testing
Unit testing is a type of automated testing meant to verify whether a small and isolated piece of the codebase—the so-called “unit”—behaves as the developer intended. An individual unit test—a “test case”—consists of an excerpt of code that exercises the production code in some way, and then verifies whether the result matches what was expected. So, unlike UI tests, unit tests don’t exercise the user interface at all; they’re supposed to interact directly with the underlying API.

Among all types of testing—manual or automated—unit testing is definitely a unique case. Most types of testing have the final user or stakeholder as the target audience, so to speak. These types of tests serve as “evidence” that the users’ requirements were met.

Unit tests, on the other hand, are different. Developers both write and read them, not with the final user in mind. Instead, developers write these kinds of tests as a check to see if the work they wrote does what they were aiming for. Having a comprehensive suite of unit tests in place allows developers to code more confidently because they feel protected by the safety net of tests.

Unit Tests Rules
Up until now, we’ve figured out some essential properties of unit tests. We express unit tests using code, unlike more visual types of tests. Also, developers are both their creators and main consumers, unlike other types of tests (such as acceptance testing) which target final users or stakeholders.


A test is not a unit test if:

It talks to the database
It communicates across the network
It touches the file system
It can’t run at the same time as any of your other unit tests
You have to do special things to your environment (such as editing config files) to run it
