# 1. What is React?

It is a JavaScript library to build User Interfaces.

​	a. React apps run in the browser. Not in the server.

​	b. In React, we create Components to create user interfaces.



# 2. What is a Component in React?

​	a. It is a custom HTML element which can be reused in React. 

​	b. A Button component, a list component, a header component etc.

​	c. We divide a complex UI into smaller independent units called Components.

​	d. React is all about Components.



# 3. How to write React code in normal HTML?

1. Import two packages, **React** & **ReactDOM** into the project.
2. Change the **Babel** pre-processor.
3. Create an element in HTML with some ID.
4. Create a function in JS file with some name and return some HTML code from this function.
5. Render this function using **ReactDOM.render()** function.

![image-20210102195543314](C:\Users\Prajwal\AppData\Roaming\Typora\typora-user-images\image-20210102195543314.png)



# 4. Why to use React?

1. UI State becomes difficult to manage with Vanilla JS in big projects. React helps here.
2. React helps us to focus on Business Logic and not on the app.
3. Huge ecosystem, active community and High Performance.



# 5. What are the alternatives of React?

1. Angular
2. Vue



# 6. What are the different type of applications?

1. **Single Page Applications (SPA)**

   a. Only one HTML page.

   b. Content is re-rendered on the HTML page again & again.

   c. Only one ReactDOM.render() method call.

2. **Multi Page Applications**

   a. Multiple HTML pages sent by Server.

   b. Content is rendered once on the server.

   c. One ReactDOM.render() call for each & every widget.