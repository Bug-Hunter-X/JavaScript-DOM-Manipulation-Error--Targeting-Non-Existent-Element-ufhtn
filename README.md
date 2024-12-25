# Uncommon HTML/JavaScript Bug: Silent DOM Manipulation Failure

This repository demonstrates a subtle bug that can occur when JavaScript code attempts to interact with a DOM element that does not exist in the HTML.  The issue lies in the attempt to modify the `style.display` property of a non-existent element, which results in a silent failure—no error is thrown, and the code continues to execute without any obvious indication of the problem.

The `bug.html` file shows the erroneous code.  The `bugSolution.html` demonstrates the corrected version, which includes a check to ensure the element exists before attempting to modify it.

This type of bug can be particularly difficult to debug because it doesn't produce a readily apparent error message.  Robust error handling and careful DOM element validation are crucial for preventing such issues.
