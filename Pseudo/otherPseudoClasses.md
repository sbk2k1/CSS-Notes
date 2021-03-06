# 1. :is() (:matches(), :any())

The :is() CSS pseudo-class function takes a selector list as its argument, and selects any element that can be
selected by one of the selectors in that list. This is useful for writing large selectors in a more compact form.

____________________________________________________________________
Selects any paragraph inside a header, main
or footer element that is being hovered 

:is(header, main, footer) p:hover {

color: red;

cursor: pointer;

}
____________________________________________________________________

 The above is equivalent to the following 

header p:hover,

main p:hover,

footer p:hover {

color: red;
cursor: pointer;
}
____________________________________________________________________

Pseudo-elements are not valid in the selector list for :is().
