# implement List.indexOf

`while`-style and recursive implementations at the top of
OrderedList_inArraySlots.java

[Java API on the `indexOf` method](https://docs.oracle.com/javase/10/docs/api/java/util/List.html#indexOf(java.lang.Object))

based on [solutionsHolmes/5D_genericTypes/OrderedList_inArraySlots_v2/](https://github.com/stuyvesant-cs/solutionsHolmes/tree/master/5D_genericTypes/OrderedList_inArraySlots_v2)
as of 2019-04-10 04:48

Logarithms
The term y = log(2)(x) refers to the idea that 2 raised to y is equal to x.
The graph begins as a concave down curve that slowly decreases in slope to 0.

The problem is finding the index in a sorted list of n length.
When I am asked to find the index of an object in a sorted list of n length, the recursive abstraction
can find the index of an object in a sorted list of n/2 length.

Boolean: When the lowest index is greater than the highest index

Base case: When the lowest index is equal to the highest index

Recursive case: There are two recursive cases;

If the index is lower then search from the lowest index to the current index - 1

If the index is higher then search from the current index + 1 to the highest index

There is no concatenation involved.

There are also no leftovers.

All that matters is the check for if the current index is equal to the item being searched for.

