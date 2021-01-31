### Lab 4 Part 1

- 1\) The length of the `prices` array gets printed because variables initialized with `var` in loops are still in the scope of the function, and after the loop ends the value of `i` is equal to the length of the prices array.

- 2\) The `discountedPrice` of the last element in the `prices` array gets printed because variables declared with `var` in loops are still scoped in the function and at line 12 `discountedPrice` gets logged after the loop ends so it is the `discountedPrice` of the last element in `prices`.

- 3\) The `finalPrice` of the last element in the `prices` array gets printed because it is declared with `var` and is scoped in the function and at line 12 `finalPrice` gets logged after the loop ends so it is the `finalPrice` of the last element in `prices`.

- 4\) `[50, 100, 150]` because the function iterates through the original array which had values 100, 200, 300 and multiplies the value by (1 - 0.5) which basically halves the inputs, and pushes it into a new array which is returned. 

- 5\) A ReferenceError is thrown because `i` was defined with `let` and has scope of within the loop, so accessing it outside the loop like in line 11 will error out.

- 6\) A ReferenceError is thrown because `discountedPrice` was defined with `let` and has scope of within the loop, so accessing it outside the loop like in line 12 will error out.

- 7\) The `finalPrice` of the last element in the `prices` array gets printed because the variable is declared with `let` and is scoped to the block, which gets set to the last element in the `prices` array after the loop ends, and will therefore be able to be printed by line 13 because it is within the same scope.

- 8\) `[50, 100, 150]` because the function iterates through the original array which had values 100, 200, 300 and multiplies the value by (1 - 0.5) which basically halves the inputs, and pushes it into a new array which is returned. 

- 9\) Even though a variable declared with `const` was reassigned in line 7 which would throw an error, assuming that was successful line 11 would throw a ReferenceError because `i` was defined with `let` and has scope of within the loop, so accessing it outside the loop like in line 11 will error out.

- 10\) Even though a variable declared with `const` was reassigned in line 7 which would throw an error, assuming that was successful line 12 would throw a ReferenceError because `discountedPrice` was defined with `const` and has scope of within the loop, so accessing it outside the loop like in line 12 will error out.

- 11\) Even though a variable declared with `const` was reassigned in line 7 which would throw an error, assuming that was successful the `finalPrice` of the last element in the `prices` array gets printed because the variable is declared with `const` and is scoped to the block, which gets set to the last element in the `prices` array after the loop ends, and will therefore be able to be printed by line 13 because it is within the same scope.

- 12\) Even though a variable declared with `const` was reassigned in line 7 which would throw an error, assuming that was successful the function would return `[50, 100, 150]` because the function iterates through the original array which had values 100, 200, 300 and multiplies the value by (1 - 0.5) which basically halves the inputs, and pushes it into a new array which is returned. An array declared with `const` can still have elements pushed into it so that would not throw an error.

- 13
  - A) `student.name`
  - B) `student['Grad Year']`
  - C) `student.greeting()`
  - D) `student['Favorite Teacher'].name`
  - E) `student.courseLoad[0]`

- 14
  - A) `'32'`
  - This is because when either of the operands in a + operation is a string, the other one is also converted to a string and both are string concatenated.
  - B) `1` because all arithmetic operators (besides addition) convert the operands to numbers before evaluation.
  - C) `3` since neither operand is a string they are converted to numbers before evaluation and the number version of null is 0.
  - D) `'3null'` since one of the operands is a string, both are converted to strings and the string version of null is 'null' and the operands are concatenated.
  - E) `4` because neither operands are strings they are converted to numbers and the number value of true is 1 and 1 + 3 is 4.
  - F) `0` because neither operands are strings, the number value of false is 0, and the number value of null is 0, 0 + 0 is 0.
  - G) `'3undefined'` because '3' is a string so the string version of undefined, which is just 'undefined' is concatenated to it.
  - H) `NaN` since both operands are converted to numbers but the number value of undefined is Nan, 3 - NaN is also NaN.

- 15
  - A) `true` because '2' and 1 are different types, they are converted to numbers and 2 > 1 so it is therefore true.
  - B) `false` because '2' and '12' are the same type(string) they are compared by lexicographical order and '2' is bigger than '12' lexicographically and the statement is therefore false.
  - C) `true` because 2 and '2' are different types, they are converted to numbers and 2 == 2 so it is therefore true.
  - D) `false` because === doesn't convert types and since 2 and '2' are different types, it is false.
  - E) `false` because true and 2 are different types, true gets converted to a number which is 1, and 1 == 2 is false.
  - F) `true` because Boolean(2) evaluates to true, and true and true are the same type and value so it is therefore true.

- 16\) `==` checks for equality of different types by converting it to a number, while `===` checks for equality without type conversion, so different types cannot be equal.

- 17\) `'How are you?'` because the first conditional is false(since different types are being compared, true becomes 1 and 1 == 2 is false) it goes to the second conditional, which is true because Boolean(2) is true, so it prints 'How are you?'.

- 19\) `[6, 8, 10]` because doSomething takes a number and function, and returns the function with input number + 2. Since modifyArray iterates through the input array and pushes the output of running the input function (callback) which is doSomething in this case, and the input function into doSomething multiplies the input by 2, the result is the number in the array, added by 2, multiplied by 2 which results in 6, 8, and 10.

- 21
  ```
  1
  4
  3
  2
  ```

