### Component Design

We've talked about composition which means in essense building blocks. So how we do the same thing for any layout?.

### Primites

Any language has primitives like an alphabetic in a human language. We use each char to form a word and this word will form a phase and so on. So why we do not do that on the layout itself?. Because we tend to think globally and give a summarise of what this big thing is like a dialog box we see the dialog not their parts. Therefore every part is attach to the dialog due dialog is the center and the unique element, something meaningul.

> A primitive is something without meaning or purpose, we use **composition** to make something meainful.

Some primitives are an input, box, label, button...etc.

So a diaglog would be a representation of primitives living in dialog context. `Box + Text + Button`. You probably cannot create literally every layout using Every Layout's primitives alone. In any case, you should walk away with an understanding and appreciation for the benefits of composition, and the power to create all sorts of interfaces with just a little reusable code.

### Responsibility

I like to keep styles separated from the parts of the app that are tied to state. That means routes, views, containers, forms, layouts, etc. should not have any styling or classes in them. Each UI component based on that encapsulates its own styling, and the styling simply becomes an implementation detail, which means a UI component can be updated or refactored without affecting anything else in the application.

Let's dive into who is responsible for what using the box model for components.

The children primitives are responsable for his of spacing (border, padding and content).
The parent primitives are responsible for the margin and position of his children.

We can distinguish two kind of primitives:

- Skeleton primitive (Button)
- Mutation/avatar primitive (ButtonBig, ButtonSecondary)

This pattern lends itself well to layout components as well. Giving a name convention for what the avatar represents there is less error prone, code duplicate and enhance reusability.

### Useful links

https://every-layout.dev/blog/algorithmic-design/

I’m sure there are even more ways to create more beautiful, more flexible, and more maintainable visual design systems.
