# bitcoin-data-cs-prep

Questions 

Let's use higher order functions like map, filter, and reduce to gather information and manipulate some data. Here we are importing historical Bitcoin data from 2013 to 2015. Each object contains information like price, market cap, fees, and much more. Let’s see what information we can extract using higher order functions!

To begin scroll down to line 8034 - click and drag the scrollbar that appears on the right as you begin scrolling to get there quickly.

First, let's log the bitcoinData object to investigate the structure of our data.

What is the data type of bitcoinData? Let’s say we just want to look at bitcoin information on May 1st, 2013. How can we do that?

Let’s say we want to create an array containing only the date and price of each day. Use the built-in map method to create an array containing that information.

Let’s create an array that only includes days when exchange volume was not 0. Which method should we use?
Everyday, new Bitcoins are generated. If we want to find out how many were generated all together during the time that’s provided in the dataset, can you figure out how to calculate it using reduce?

Bitcoin price fluctuates a lot. Let’s combine some array methods to find the total number of days when bitcoin price was over $100!
And finally, let’s find the average bitcoin transaction fees between 2013 and 2015. Be sure to floor this value.

## Bonus Challenges
Move onto these challenges only if you have finished the main challenges

1. dayMapper (follow up to challenge 3)

- Write a function called dayMapper. It will accept three parameters: arr (bitcoinData), property1, property2.
- It should use map to return a new array of objects with only the passed in properties on each object.
- If the passed in properties are not present in arr's objects, then it should ignore that property name and it should not appear in the returned array.
2. averageValueOf________ (follow up to challenge 7)

- for each property that has numeric values in bitcoin data, write a function that takes in an array (bitcoinData in this case) and a property name and will return the property's average value in the array.
3. averageValueBonus (double follow up to challenge 7)

- write a function called generalAverageValue that takes two parameters: arr and property.
- arr will be bitcoinData and property will be a property name from the array of objets.
- your function should check to make sure that property's values are numeric. if they're not, it should return an error message of your choosing. If you'd like, you can research throw new Error() and do that instead
- your function should return an array of the form [property, avgValue]
4. Tally bitcoin prices by range

- write a function called priceRangeTally which accepts one argument, arr. Your function should do the following:
- find the maximum bitcoin price
- find the minimum bitcoin price
- choose an arbitrary interval to create ranges (you can do this dynamically or hard code it, up to you)
- Tally how many days of bitcoin prices fall into each range
- console.log a nicely formatted string of each interval and how many days fall into each interval.
- you don't have to return anything, but you can return a tally object or array of your choosing.
5. write a function that will accept an array (bitcoin data) as a param, and return an object with keys that are the names of all the numerical properties of the bitcoindata objects, and whose values are the max values of those properties

5.5. do the same thing, but for minimum values

6. write a function that compares the two objects from number 5 and creates a new object with the same keys, but the values are the ranges of Max - Min
