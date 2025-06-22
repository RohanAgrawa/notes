1. Server Component :-

We can implement react component similar in next js, but this is not a normal react component instead its React server component, because its executed in server not on client machine.

It store logs on server instead of browser console.

![image](https://github.com/user-attachments/assets/ef7e0bc5-3b28-4242-9c60-76ce0a0118bb)

2. SPA:-
     React is by default single page application and it executes at client side machine javascript code. In Next JS code executes on server instead of client machine when we change or update the route manually through browser we can see the page is being reloaded and previous page we have been left. To work with SPA in next js we use Link tag which provided by this framework to route to different page without reloding the page, still page is executed at server but it updates the client or browser javascript code to work with SPA as we do with React Application from ages.

Basically Next JS is we can do both.

3. Routes :-
     In React we use React Router package to routes or navigate accross application with the help of createBrowserRoute but here in Next JS we can route based on file sytem we don't need any extra dependency installation, Just we need to setup the folder and files inside app folder which is main folder and page.js is default name that next.js detects and renders and executes to server.

![image](https://github.com/user-attachments/assets/32651784-b3d4-440a-a7e5-59f03fada03c)
![image](https://github.com/user-attachments/assets/8596e673-5fe3-4754-8ea9-c219901268cb)

4. layout.js :-
     layout.js is file is wrapper for the childerens means the components or pages.js are being rendered inside it.
        Childeren property is the current childeren that is executed or present inide the layout.js
   In a project at least one layout.js is mandatory but we can different layout.js in different folders depending on the situation, layout.js is by default a reserverd name in next.js just like page.js

     To add a meta data about the page we use meta data object that is also reserverd name in layout.js that gives information about page similar like <head> we use in normal HTML head tag.

   ![image](https://github.com/user-attachments/assets/fb78fa51-a294-470b-87db-4354a359a1e2)
     ![image](https://github.com/user-attachments/assets/d216684d-984d-447c-aef0-65c85ade15ed)



