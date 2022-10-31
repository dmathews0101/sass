# sass-12-if-statements

1. using @if statements in sass
2. if statements are controlled flow statements, whereby we say if something occurs or rather if a condition is true, then do something
3. we can apply the same logic to sass to apply styles depending on certain conditions
4. mixin with more than one argument : 
@mixin mQ($arg...){
    @if length($arg) == 1{
        @media screen and (max-width: nth($arg, 1)){
            @content;
        }
    }
    @if length($arg) == 2{
        @media screen and (max-width: nth($arg, 1)) and (min-width: nth($arg, 2)){
            @content;
        }
    }    
}