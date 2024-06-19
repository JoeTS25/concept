### Conceptual Exercise

Answer the following questions below:

- What is the purpose of the React Router?
To use different route components and group them all together under a Routes tag

- What is a single page application?
Sites that exclusively use client-side routing (handles mapping between URL bar and page user sees
via browser rather than via server)

- What are some differences between client side and server side routing?
Server side routing: server decides what HTML to return based on URL requested (different pages load)
Client side shows and hides content depending on where you are (single page app)

- What are two ways of handling redirects with React Router? When would you use each?
<Redirect> component: useful for redirecting away from page that should not have been accessed
Calling ".push" method on history object: useful for handling logic then redirecting

- What are two different ways to handle page-not-found user experiences using React Router? 
Add route at bottom of Switch <Route><NotFound /></Route>(catch all)

- How do you grab URL parameters from within a component using React Router?
You use "useParams" hook (const params = useParams();). "params" is an object that contains variables
from the route. 

Example: Route path = "/food/:name" (the ":" means it's a variable). 
Then in the component function: const params = useParams();
You are now able to use { params.name } to account for any user's variable

- What is context in React? When would you use it?
Context is universal data across app. Useful for prop drilling, less repitition 

- Describe some differences between class-based components and function
  components in React.
Class components must have a render method describing what the component should render.
Every component extends React.Component.

Function components let you use React without classes via hooks

- What are some of the problems that hooks were designed to solve?
Hooks let you use state and other React features without writing a class.
Hooks let you "hook into" React state and lifecycle features from function components