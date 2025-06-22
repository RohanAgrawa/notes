1. Server Component :-

We can implement react component similar in next js, but this is not a normal react component instead its React server component, because its executed in server not on client machine.

It store logs on server instead of browser console.

![image](https://github.com/user-attachments/assets/ef7e0bc5-3b28-4242-9c60-76ce0a0118bb)

-----------------------------------------------------------------------------------------------------------------------------------------------------

2. SPA:-
     React is by default single page application and it executes at client side machine javascript code. In Next JS code executes on server instead of client machine when we change or update the route manually through browser we can see the page is being reloaded and previous page we have been left. To work with SPA in next js we use Link tag which provided by this framework to route to different page without reloding the page, still page is executed at server but it updates the client or browser javascript code to work with SPA as we do with React Application from ages.

Basically Next JS is we can do both.

-----------------------------------------------------------------------------------------------------------------------------------------------------

3. Routes :-
     In React we use React Router package to routes or navigate accross application with the help of createBrowserRoute but here in Next JS we can route based on file sytem we don't need any extra dependency installation, Just we need to setup the folder and files inside app folder which is main folder and page.js is default name that next.js detects and renders and executes to server.

![image](https://github.com/user-attachments/assets/32651784-b3d4-440a-a7e5-59f03fada03c)
![image](https://github.com/user-attachments/assets/8596e673-5fe3-4754-8ea9-c219901268cb)

-----------------------------------------------------------------------------------------------------------------------------------------------------

4. layout.js :-
     layout.js is file is wrapper for the childerens means the components or pages.js are being rendered inside it.
        Childeren property is the current childeren that is executed or present inide the layout.js
   In a project at least one layout.js is mandatory but we can different layout.js in different folders depending on the situation, layout.js is by default a reserverd name in next.js just like page.js

     To add a meta data about the page we use meta data object that is also reserverd name in layout.js that gives information about page similar like <head> we use in normal HTML head tag.

   ![image](https://github.com/user-attachments/assets/fb78fa51-a294-470b-87db-4354a359a1e2)
     ![image](https://github.com/user-attachments/assets/d216684d-984d-447c-aef0-65c85ade15ed)

not-found.js => Fallback page for "Not Found" errors (thrown by sibling or nested pages or layouts)

error.js => Fallback page for other errors (thrown by sibling pages or nested pages or layouts)

loading.js => Fallback page which is shown whilst sibling or nested pages (or layouts) are fetching data

route.js => Allows you to create an API route (i.e., a page which does NOT return JSX code but instead data, e.g., in the JSON format)

-----------------------------------------------------------------------------------------------------------------------------------------------------

5. global.css & icon.png :-
        global.css is another reserverd file name wich contains a css that can be used globally in application and its imported in layout.js because its wrapper for the childerens.

   icon.png is also reserver file name and if we use this name next js will treat this as fav icon and you can see the fav icon on your browser tab.

![image](https://github.com/user-attachments/assets/c9b69705-6af9-439e-a96f-9b1ecad5f100)
![image](https://github.com/user-attachments/assets/55466ca2-c7c1-4370-83b4-5109f473b080)

-----------------------------------------------------------------------------------------------------------------------------------------------------

6. Vanilla React Component Concept :-
        In React we create a seprate component for the specific task to perform but here in Next.js we have reserverd file page.js that executes the component on server but that file can be very long and and bulky that doesn't make sense to write everything in it.

To overcome this problem we can use vanila react component concept in we write different component and name the file according to the task we want to perform in that file. But next.js will not automatically detect and execute because that's not reserver name for execution and routing. But to notify next js about the components we can import in page.js and export from component from file in which we created.

![image](https://github.com/user-attachments/assets/bd7b5783-7113-4ea4-8899-0c233a318890)

Most preferd way is to keep the component folder is outside of app folder because it is not part of reserverd names in files systems and Next App routes.

while importing we can use @ also to refer to the root level directly instead of following directory hierarchy.

![image](https://github.com/user-attachments/assets/b083ca14-6a1e-40d7-9b4d-df4865d4a496)

-----------------------------------------------------------------------------------------------------------------------------------------------------

7. Dynamic Routes :-

     Dynamic Routes is very important concepte for UI, suppose we to routes to a different page but the content is dynamic dependes on data from backend or other source. To create a dynamic routes we will create a folder with [] square brackets and inside that brackets just add any name as place holder. Inside this special folder we will create page.js that will render the dynamic route page.

To verify the how is it dynamic next js pass a param props to the special folder page.js component which contains the detail of dynamic route.

![image](https://github.com/user-attachments/assets/aec9617c-28b8-4c2c-8ee3-2ebab6c936ae)
![image](https://github.com/user-attachments/assets/ef8872ca-d216-40f9-bd65-f63478b25c4b)
![image](https://github.com/user-attachments/assets/545b0050-4d7c-407e-b93e-e8ef60204c36)




