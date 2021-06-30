## React 3


***Why Next.js ?*** 

**A framework can solve these problems. But such a framework must have the right level of abstraction — otherwise it won’t be very useful. It also needs to have great "Developer Experience", ensuring you and your team have an amazing experience while writing code.**

- I might want to statically pre-render some pages for performance and SEO. I might also want to use server-side rendering or client-side rendering.

- I might have to write some server-side code to connect your React app to your data store.

***Next.js: The React Framework***
**Next.js provides a solution to all of the above problems. But more importantly, it puts you and your team in the pit of success when building React applications.**

**Create a Next.js app**
To create a Next.js app run the following command:

npx create-next-app 



**Run the development server**
cd nextjs-blog

***Then, run the following command:***
npm run dev


## Assets, Metadata, and CSS

**Assets**

-  We have to manually handle to Ensuring your image is responsive on different screen sizes. Optimizing your images with a third-party tool or library and Only loading images when they enter the viewport.


- Next.js can serve static assets, like images, under the top-level public directory. Files inside public can be referenced from the root of the application similar to pages.

- The public directory is also useful for robots.txt, Google Site Verification, and any other static assets.


**Metadata**
Modify the metadata of the page, such as the <title> HTML tag

- <title> is part of the <head> HTML tag, so let's dive into how we can modify the <head> tag in a Next.js page.


**CSS Styling**

- The index page already has some styles. 
- This page is using a library called styled-jsx. It’s a “CSS-in-JS” library — it lets you write CSS within a React component
