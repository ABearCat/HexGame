# HexGame
Hexagon based game where you remove "lines"

A line in this game will be any where any 2 opposing edge pieces as well as all the pieces in between have been filled in, they will all be cleared.

The board will be represented in an array of this size, where the only locations that can hold pieces will be marked off with an X
```
[x] [x] [x] [x] [x] [ ] [ ] [ ] [ ]
[x] [x] [x] [x] [x] [x] [ ] [ ] [ ]
[x] [x] [x] [x] [x] [x] [x] [ ] [ ]
[x] [x] [x] [x] [x] [x] [x] [x] [ ]
[x] [x] [x] [x] [x] [x] [x] [x] [x]
[ ] [x] [x] [x] [x] [x] [x] [x] [x]
[ ] [ ] [x] [x] [x] [x] [x] [x] [x]
[ ] [ ] [ ] [x] [x] [x] [x] [x] [x]
[ ] [ ] [ ] [ ] [x] [x] [x] [x] [x]
```

This array is meant to represent a hexagon regular hexagon that is 5 units wide on any edge, as a result a successful line clear will involve either fully filling out any of the rows (including short rows), columns (including short columns) and right leaning diagonals.
At any point, there would be 27 potential lines that could be filled out. This project will first be written in a simple manner designed to just iterate through all 27 in order to find any completed lines, whereas the later version will only check the lines surrounding the piece most recently placed.
