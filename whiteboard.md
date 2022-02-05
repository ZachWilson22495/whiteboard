function dupeKiller(array) {
  if (newArray <= 1) {
    return uniqueArray;
  } else if (!uniqueArray.includes(array[0])) {
    uniqueArray.push(array[0]) + dupeKiller(newArray = (array.substring(1, array.length)))
  } else if (uniqueArray.includes(array[0])) {
    dupekiller(newArray = (array.substring(1, array.length)))
  }
}

function dupeKiller(array) => { return uniqueArray.from(new Set(array)) }




<!-- -Take in an array

-examine the first element of the array

-push first element to 'dupeArray' if identical element does not already exist within 'dupeArray'

-return dupeArray


----------------------------------------------------------------------------------------------------


Question #2: Array Deduping
Write an algorithm that removes duplicates from an array. Do not use a function like filter() to solve this. Once you have solved the problem, demonstrate how it can be solved with filter(). Solve the problem with and without recursion.

Example
Input: [7, 9, "hi", 12, "hi" 7, 53]

Output: [7, 9, "hi", 12, 53] -->