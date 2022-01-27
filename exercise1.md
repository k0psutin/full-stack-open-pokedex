Some common steps in a CI setup include linting, testing, and building. What are the specific tools for taking care of these steps in the ecosystem of the language you picked? 

Example if the project is in Java, you can use checkstyle for linting, and there are GitHub Actions for automating the processes for checkstyle. That way you can fail the CI pipeline if there are any errors.

Java has several package managers, Maven and Gradle for example, and you can use them from the GitHub Actions command line to test and build the code. Alternative to the GitHub actions would be for example Travis CI. Travis CI is a commercial pipeline. There is also Circle CI. 

- Would this setup be better in a self-hosted or a cloud-based environment? Why? What information would you need to make that decision?

It is hard to say. If you have a large scale project with multiple developers, then I would say the cloud-based environment is the best, since there are a lot of variation on operating systems and hardware.

But if you have a small team, then you could probably manage it locally via Jenkins or other CI automation software.