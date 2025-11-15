

📚 Regular Expressions in Linux (Regex in Linux)

Date: November 15, 2025  
Level: Intermediate  
Status: 🟢 Completed

---

🎯 Goals

* Understand how to search for specific patterns inside files using regular expressions.
* Gain practical skills in using grep, awk, and sed to filter and analyze data accurately.

---

📝 Summary & Core Concepts

Regular expressions (Regex) are a powerful tool for searching, validating, and extracting patterns from text. They are used in tools like grep, awk, and even programming languages. Regex is a fundamental part of file analysis in Linux.

📑 Key Concepts
* Regex: A syntax for defining specific text patterns.
* grep -E: A command-line tool for searching using extended regular expressions.

---

⚙️ Practical Commands & Examples

1. Grouping with Parentheses

Description: Parentheses are used to group parts of a pattern, specify repetition, or define character classes.

| Description                                                 | Operator |
| ----------------------------------------------------------- | -------- |
| Group parts of an expression                                | (a)    |
| Define character classes (e.g., from a to z)                | [a-z]  |
| Specify repetition count                                    | {1,10} |
| OR operator (matches if either expression is true)          | \|     |
| Approximate AND (requires both patterns in order)           | .*     |

---

2. Difference Between OR and AND in Regex

🔸 OR – Either one is enough:
`bash
grep -E "(my|false)" /etc/passwd
`
Displays any line containing "my" or "false" or both.

🔸 AND – Both together:
`bash
grep -E "(my.*false)" /etc/passwd
`
Displays only lines containing "my" followed by "false" in the same order.

🔸 Alternative AND method:
`bash
grep -E "my" /etc/passwd | grep -E "false"
`
Meaning: First search for "my", then filter results that also contain "false".

---

📊 Outcomes & Key Takeaways

* Positive Outcome: Learned how to use grep to filter data precisely with combined patterns.  
 Challenge Faced: Understanding the difference between | and . in expressions, solved through practice.  
* Key Lesson: Regex is not just symbols—it’s a logical search system that saves time and effort in file analysis.

---

🔗 Keywords & Resources

🏷️ Keywords
Linux, Regex, grep, awk, sed, CybersecurityTools, TextProcessing

📚 Further Reading
1. Regex Tutorial - Learn by Examples  
2. Linux grep Command Guide
