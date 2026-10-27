| Bug | Evidence / Failed Test | Cause | Fix |
| :--- | :--- | :--- | :--- |
| Average | 135.0 instead of 90.0; singlemark crash | Dividing by len(marks) - 1 | Divide by len(marks) |
| Pass boundary | 40 returned False | Used > instead of >= | Use >= PASS_MARK |
| Distinction | 95 returned First | >=60 checked before >=90 | Check >=90 first |