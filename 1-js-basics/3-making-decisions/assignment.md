# Operators
```javascript
let allStudents = [
  'A',
  'B-',
  1,
  4,
  5,
  2
]

let studentsWhoPass = [];
for (let i = 0; i < allStudents.length; i++) {
  let grade = allStudents[i];
  if (typeof grade === "number") {
    if (grade >= 3) {
      studentsWhoPass.push(grade);
    }
  }

  else if (typeof grade === "string") {
    if (grade === "A" || grade === "A-" || grade === "B" || 
        grade === "B-" || grade === "C" || grade === "C-") {
      studentsWhoPass.push(grade);
    }
  }
}
console.log("Passing Students:", studentsWhoPass);
```
