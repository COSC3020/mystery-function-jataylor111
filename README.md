[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-718a45dd9cf7e7f842a935f5ebbe5719a5e09af4491e668f4dbf3b35d5cca122.svg)](https://classroom.github.com/online_ide?assignment_repo_id=11752240&assignment_repo_type=AssignmentRepo)
# Mystery Function

What does the `mystery()` function in the following piece of code do? Add your
answer to this markdown file.

```javascript
function mystery(a) {
    if(a.length == 1) return a[0];
    var foo = mystery(a.slice(1, a.length))
    if(foo > a[0]) return foo;
    else return a[0];
}
```
This function takes the array 'a' and first checks to see if it only has a a length of 1, if it does it just returns the first entry, 
if not it creates the variable foo and it is built by taking a slice of the array a, starting at 1, and keeps "looping" through the function shrinking 
foo until foo is a single entry, it then compares that final entry with a[0], and if foo is larger it returns foo, if not it just returns a[0].
