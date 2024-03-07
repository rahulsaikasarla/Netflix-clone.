Logo
Netflix Clone
View Demo · Report Bug · Request Feature

Table of Contents

Logo
Home Page

Logo
Mini Portal

Logo
Detail Modal

Logo
Grid Genre Page

Logo
Watch Page with customer contol bar

Prerequests
Create an account if you don't have on TMDB. Because I use its free API to consume movie/tv data.
And then follow the documentation to create API Key
Finally, if you use v3 of TMDB API, create a file named .env, and copy and paste the content of .env.example. And then paste the API Key you just created.
Which features this project deal with
How to create and use Custom Hooks
How to use Context and its provider
How to use lazy and Suspense for Code-Splitting
How to use a new lazy feature of react-router to reduce bundle size.
How to use data loader of react-router, and how to use redux dispatch in the loader to fetch data before rendering component.
How to use Portal
How to use Fowarding Refs to make components reusuable
How to create and use HOC
How to customize default theme of MUI
How to use RTK
How to use RTK Query
How to customize default classname of MUI
Infinite Scrolling(using Intersection Observer API)
How to make awesome carousel using slick-carousel
Third Party libraries used except for React and RTK
react-router-dom@v6.9
MUI(Material UI)
framer-motion
video.js
react-slick
Install with Docker
docker build --build-arg TMDB_V3_API_KEY=your_api_key_here -t netflix-clone .

docker run --name netflix-clone-website --rm -d -p 80:80 netflix-clone
Todo
Make the animation of video card portal more similar to Netflix.
Improve performance. I am using context and provider but all components subscribed to the context's value are re-rendered. These re-renders happen even if the part of the value is not used in render of the component. there are several ways to prevent the re-renders from these behaviours. In addition to them, there may be several performance issues.
Replace bundler(Vite) with Turbopack. Turbopack is introduced in Next.js conf recently. It's very fast but it's nor ready to use right now. it just support Next.js, and they plan to support all others as soon as possible. so if it's ready to use, replace Vite with Turbopack.
Add accessibilities for better UX.
Add Tests.
