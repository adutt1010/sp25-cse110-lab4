1. values added:  20  
2. final result:  20  
3. You should not use `var` because it is function-scoped instead of block-scoped. This can lead to bugs where variables are unintentionally accessed or modified outside the block where they were defined. `let` and `const` are block-scoped and provide more predictable behavior.
4. values added:  20  
5. ReferenceError: result is not defined  
Line 13 is outside the block where `result` was declared using `let`. Since `let` is block-scoped, this results in a ReferenceError.
6. TypeError: Assignment to constant variable.  
`result` is declared with `const` and given the value 0. The next line tries to reassign it to `num1 + num2`, which is not allowed with `const`, resulting in a TypeError.
7. Nothing is printed.  
The error on line 7 prevents execution from reaching line 13. Even if it did, it would throw a ReferenceError because `result` is block-scoped and not accessible there.
