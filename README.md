1)When I add items to my cart, everything works. Then if I go to the cart page the cart is empty.

So in your app.js file, line 24, you need to change the code to( localStorage.setItem("cart", JSON.stringify(this.items)); )
You are attempting to save the cart items to localStorage, but you are referencing this.item (singular) instead of this.items which is a common mistake.

2)Have best practices been followed?
    While some best practices have been followed such as using constructor functions, Prototypes or descriptive Variable Names, 
    I believe there are opportunities for improvement.


3)What would you recommend they do to extend this?

You can consider optimizing the code for performance by minimizing DOM manipulation or bundling and minifying JavaScript files for production.
If you have repetitive code, consider creating functions or loops or caching elements in variables to handle similar tasks.
For example, when creating products, you could use a loop.