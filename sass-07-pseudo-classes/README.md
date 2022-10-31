# sass-07-pseudo-classes

1. using pseudo classes in sass
2. in css we use pseudo classes to add in extra effects such as hover effects, or we can use them to  insert content after,.. syntax: :pseudo-class
3. for example, if we want to add an hover effect to the links at the top,.. in css,
#main-nav a:hover{
    background: #333;
}
4. in sass, .. we have to use &..
a{
    color: $offWhite;
    ...
    &:hover{
        background: #333;
    }
}