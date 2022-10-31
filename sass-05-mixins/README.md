# sass-05-mixins

1. at its most basic form, a mixin is a chunk of reusable css or sass, that we can just inject into any element that we want
2. for example, if we have different elements on our page like a tags, buttons, form elements,.. which all use a particular set of styles,.. then instead of applying all of those styles to each of those elements individually,.. 
3. what we can do is create a mixin, which creates all of those styles or nesting styles,.. and then we can import that mixin into whichever elements require those styles,.. can save time
4. we can also pass through variables or arguments to those mixins, from these different elements that we are styling up, and thats gonna possibly change the output of those mixins, depending on the element that is calling them