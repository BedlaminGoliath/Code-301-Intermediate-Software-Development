# Components

1. What is a “component”?

- This is a “modular” block or blocks of functionality, that is well defined and easy to use and read. This usually comes in the form of a software object. These play well with other components (pieces of the same shelf being built). These hold a standard to which they are easily pliable and can build bigger things of wanted.

 -Can have 3 views :
-object-oriented [a set of classes that work well together,  each class and design are “defined” to identify all attr. And oper. That they are being used for.

-conventional view : a functional element / module of program that integrates processing logic. Alll internal data structures that is required as well as interfaces.

-process-related view: These use pre-existing components, that come from a library, While components are being formulated, components are being picked from the library.

- a UI uses grids, buttons, and utility pieces

1. What are the characteristics of a component?

- Reusable :throughout the code.
- Replaceable: by other components
- Non context specific specific: these can operate in different environments
- Extensible - you can add pieces from existing pieces to another piece to change usability / functionality.
- Independent: not much need for other pieces.

1. What are the advantages of using component-based architecture?

- It’s easy to replace existing pieces as new pieces are made because everything        “snaps” together.
- It’s cheap because you can “spread” the cost of dev. And maintenance.
- Since all pieces are reusable can be spread across the development.
- Modified complexity through the use of its “component container”
- they are reliable.
- They are easy to swap out and or update.
- These individual pieces work independently and they are flexible with connectivity from component to components.

Component based architecture leans on the decomposition  of design into basic compartmentalized functions, that make up a well defined interface. These are meant to be broke down into functions, methods, event handler, so the problems can be solved easily.  Best of component reuse-ability.
These are best used because by using preexisting components you are using pre made pieces. These are time tested and easy to use. Plug-in based architecture .

REACT:

React is a comp. based library that consists of smaller block that can be used. These UI pieces are broken down into smaller pieces.

1. What is “props” short for?

- Props stand for “properties”. these are used by way of passing data from component to component.
  - props are objects the data gets passed in one direction (parent to child). (Unidirectional flow). This data is “read only” there for this should not be changed in transit.

1. How are props used in React?

Props are objects that can be used as arguments, these props carry data and allow us to call certain props and place those props within their parent elements (components) with ease. We make use of dot notation along side the special keyword “props” so we would use the keyword “.” The attribute name that we made to carry that piece of information.

- Define an attribute and value.
- Pass it to child components by way of props
- Render the props data.

1. What is the flow of props?

- the flow of props is “one way” which is from top down or from parent to child and is read only so an error will get thrown of you try to manipulate the prop “outside of its scope….?” Im not sure if thats how you word it. Well find out.
