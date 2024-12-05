# Uncommon HTML Bug: DOM Element Access Before Page Load

This repository demonstrates a subtle bug in HTML that occurs when attempting to access and manipulate DOM elements before the page has fully loaded.  This can lead to unexpected errors or failures.

## The Bug

The `bug.html` file contains a simple HTML page with a `div` element.  A JavaScript script attempts to modify the `innerHTML` of this `div` before the page has finished loading.  This results in a runtime error because the element might not exist yet.

## The Solution

The `bugSolution.html` file presents a corrected version.  It uses the `DOMContentLoaded` event to ensure that the script executes only after the page's DOM is fully loaded and parsed, preventing the error. 

## How to Reproduce

1. Clone this repository.
2. Open `bug.html` in your web browser. You should see an error in the console.
3. Open `bugSolution.html`. This version will work correctly.