# sass-11-content

1. using content keyword in sass
2. the content keyword subs in styles from our rules and puts those styles whereever it finds the content keyword
3. making a mixin, which controls the media queries, .. keeps media queries in one place, together with the rules
4. if we wanted to change the banner at 800px, we would call this mixin on the banner element, and would pass in 800px, then it is going to set this media query for us on that element and set the max width to 800px, then we could add in our styles inside this media query,.. using @content keyword inside
@mixin mQ($arg){
    @media screen and (max-width: $arg){
        @content;
    }
}
5. thats all we need to do for this mixin, because when we call this mixin, on the element that we want to change at a particular width, then we are going to specify what content we want to pass in here
6. we pass in the width at which we want it to change, to the media query mixin
    li {
        float: left;
        width: (100% / 6);
        @include mQ(600px){
            
        }
    }
whatever we put inside the include code block, that goes into the @content section,.. that way we dont have to define it within this mixin itself,.. we can just define it on the element, and that is brought in when we use that mixin
7. we can create a really simple media query mixin which is dynamic and can insert our own content from whereever we call it