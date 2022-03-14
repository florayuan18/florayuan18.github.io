---
layout: page
title: Week 0 - Menu Code Snippets
subtitle: Flora Yuan
---
## Challenges
**Week 0 - Menu**

Challenges:
* Create alternate menu with data structure
* Swap numbers and add to Menu
* Matrix

## Code Snippets
`// Map.Entry - access entries within a map
for (Map.Entry<Integer, AltMenu> pair : menu.entrySet()) { // entrySet returns a set that has the same elements as the map, entrySet is an array, take elements out
System.out.println(pair.getKey() + " ==> " + pair.getValue().getTitle()); // printing out key and value combination
}`
* this segment of the code accesses the entries within the map.  It returns the values of the key and value combination within the HashMap.  I had to research what a HashMap was. but was eventually able to figure out the components of a HashMap.

`    public void swapToLowHighOrder(IntByReference object2) {
if (this.value > object2.value) {
int temp = this.value; // creating a temporary variable to hold this.value
this.value = object2.value; // assigning the object.value to this.value
object2.value = temp;
}
}`
* creating a temporary variable that holds the value while the values are swapped.  This was difficult to figure out because I wasn't sure how to directly swap the values, so I added in another variable to act as a median.

`for(int j = 0; j < matrix[i].length; ++j) { // checking each element of the row | when j = matrix length, moves to next row
if (matrix[i][j] == -1) { // if the value in the matrix = -1
myOutput += " "; // replace the value in the matrix with a space
}`
* code in order to replace the values within the matrix - a key aspect of the Third Challenge
* This helped me better understand how to move through a matrix and carry through actions based on the current element

## GitHub
[Challenge 1](https://github.com/florayuan18/just-to-suffer/commit/fa51cfa45fe7f2baf52cd41939b30adbe716edbf#diff-a381d0919fb872c439419597c681ac66f7118bbd4f996f621ac854da5cbf8e6cR1-R42)
[Challenge 2](https://github.com/florayuan18/just-to-suffer/commit/fa51cfa45fe7f2baf52cd41939b30adbe716edbf#diff-79d3f3c548e6fc4fe97753724d0e58c838519abac6f2028d025647dd8620badeR1-R39)
[Challenge 3](https://github.com/florayuan18/just-to-suffer/commit/fa51cfa45fe7f2baf52cd41939b30adbe716edbf#diff-679a6612cc9f2cd06dc1e3fc480923bebea7f4d13390308de88ad01fb8b744beR1-R74)

## Replit
[Replit](https://replit.com/@florayuan18/just-to-suffer#challenges/AltMenu.java)