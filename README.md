# Uncommon HTML Bug: innerHTML Performance and Security

This repository demonstrates an uncommon bug related to the use of `innerHTML` in HTML.  While seemingly innocuous, repeatedly using `innerHTML` to modify the DOM can lead to performance degradation and security risks.  This example shows the problem and provides a better solution.

## The Problem

The `bug.html` file shows the incorrect usage of `innerHTML`. Appending to `innerHTML` is inefficient and can be vulnerable to XSS attacks if the appended content is not properly sanitized. 

## The Solution

The `bugSolution.html` file presents the improved approach using `insertAdjacentHTML`. This method is generally safer and more performant for adding content to the DOM.

## How to Run

1. Clone this repository.
2. Open `bug.html` and `bugSolution.html` in your web browser to see the difference in behavior and performance.

## Conclusion

Understanding the potential issues associated with `innerHTML` is crucial for building secure and efficient web applications.  Using methods like `insertAdjacentHTML` offers a more robust approach.