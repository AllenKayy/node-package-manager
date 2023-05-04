# Module 7

## What is the Event loop?

The Event loop is a process that allows NodeJS perform non-blocking, asynchronous I/O operations. An event loop works by continuously monitoring a set of input sources, such as user input, network I/O, or file I/O, for new events or tasks to perform. When an event occurs, the event loop checks if there is a registered callback function for that event and executes it.

The event loop then moves on to the next event, repeating the process until there are no more events to process. This allows for multiple tasks to be executed in parallel without blocking the main thread of execution or requiring additional threads or processes.

## Explain the 6 phases of the event loop
The 6 phases of the event loop are:

1. Timers: This phase executes all callbacks that are scheduled to run at a particular time using setTimeout() and setInterval().

2. Pending callbacks: (Internal phase) This phase executes callbacks that were deferred by the previous iteration of the event loop.

3. Idle, prepare: This phase is used for internal purposes by Node.js.

4. Poll: This phase retrieves and processes I/O events from the system, such as incoming network data or user input.

5. Check: This phase executes callbacks that were scheduled by setImmediate().

6. Close callbacks: This phase executes callbacks that were registered to be executed when a resource, such as a socket or file handle, is closed.

##  List some best practices in server-side code development

Some best practices in server-side code development includes:

- Write modular code: Break down your code into small, reusable modules that can be easily tested, maintained, and updated. This makes your code more scalable and easier to understand.

- Use version control: Use a version control system like Git to track changes to your code, collaborate with other developers, and revert to previous versions if necessary.

- Document your code: Write clear and concise comments to explain how your code works, what it does, and any assumptions or limitations.

- Follow coding standards: Use consistent naming conventions, indentation, and formatting to make your code more readable and easier to maintain. Follow industry-standard coding practices and guidelines.

- Use error handling: Always handle errors gracefully and provide informative error messages to users. This helps you to detect and debug issues quickly, and improve the user experience.

- Secure your code: Use best practices for security, such as input validation, encryption, and authentication. Protect sensitive data and resources, and keep your software up-to-date with security patches.

- Optimize performance: Optimize your code for performance and scalability, such as minimizing database queries, caching, and using efficient algorithms. Monitor performance and use profiling tools to identify bottlenecks.

- Test your code: Test your code thoroughly, including unit tests, integration tests, and end-to-end tests. Use automated testing frameworks and continuous integration tools to improve code quality and reduce bugs.

- Use logging and monitoring: Use logging and monitoring tools to capture and analyze data about your application's behavior and performance. This helps you to identify issues and improve the user experience.

- Continuously improve: Continuously review and improve your code, based on feedback from users, stakeholders, and other developers. Stay up-to-date with new technologies and industry trends, and continuously learn and improve your skills.

## What is NPM5: How do you initialize a package in npm 

NPM5 (Node Package Manager) is a tool for managing project dependencies via command line It is used to install, manage, and share packages, which are collections of code and dependencies that can be easily installed and integrated into Node.js projects. 

Npm is an essential tool for Node.js development, enabling developers to quickly and easily add functionality to their projects using a vast array of open-source packages.

You can initialize a package in npm by running `npm init`

## How do you run a script in the package.json

You can run a script in the package.json file by running the command `npm start`
npm start
