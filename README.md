# Software Engineering Notes

## Article: The Twelve-Factor App

[The Twelve-Factor App](https://12factor.net/) describes a set of practices for building software-as-a-service applications that can run reliably across different environments.

I find the article interesting because it connects everyday engineering choices, such as keeping configuration out of code and treating backing services as replaceable resources, to the larger goal of making an application easier to deploy and maintain. These practices also give teams a shared vocabulary for discussing operational design before deployment problems appear.

The ideas are useful beyond web services. Separating environment-specific configuration and making processes reproducible can help almost any software project become easier to test, run, and hand off to another developer.


## Comment from Yusef Moustafa

I like this pick because Twelve-Factor is one of those things that sounds obvious once you have been burned by not following it, but is easy to skip when you are just trying to get something running. The point about keeping config out of code stood out to me the most since I have seen how quickly a project gets fragile once an API key or a database URL is hardcoded somewhere and then has to be hunted down later.

The point about treating backing services as replaceable resources also connects well to something I ran into during my internship, where swapping out one auditing tool for another was much easier because the team had not tightly coupled the code to a specific vendor. It made me realize these principles are less about following a checklist and more about designing for change from the start.