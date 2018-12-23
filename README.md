The Above stylesheet shows off some of the new features available with CSS3 

/* You can use specific color using rgba */
rgba(255,255,255,0.1) // last value is for the intensity of the color

/* Gradient */
linear-gradient(55deg, black,yellow)// you can specify the type of gradient witht the first value
radial-gradient(blue, yellow ,orange);

/* Shadows */
/* horizontal, vertical, blur, spread; */
box-shadow: 10px 10px #333;
box-shadow: 0 20px 10px 15px #333;

/*shadow: horizontal, vertical, color*/
/*you can set multiple shadows in css 3*/
text-shadow: 2px 2px 5px black, 2px;

/* Column 
This is a neat trick to divide text into column.
*/
column-count: 3;
column-gap: 10px;
column-rule-color: aqua;
    
// this may not work for older browsers but to be on the safe side include these commands for your specific browser
-webkit-column-count:3;
-webkit-column-rule-style: solid;
-webkit-column-rule-color: aqua;

/*Animations & Transitions 
Fist initialize a @keyframe rule
*/

@keyframes box{
    from{ border-radius: 40px; background-color: red;top:0;left:0}
    to{background-color: 40px;background-color: }
}
#animations #box{
    position: relative;
    animation-name: box;
    animation-duration: 4s;
    animation-delay: 4s;
    animation-iteration-count: 3;
    animation-direction: alternate;
    animation-timing-function: ease-in-out;
/*    shorthand version*/
/*    animation: box 10s linear 2s 3 alternate;*/
}


