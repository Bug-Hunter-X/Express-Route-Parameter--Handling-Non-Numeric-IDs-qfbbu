# Express Route Parameter: Handling Non-Numeric IDs

This repository demonstrates a common error in Express.js applications involving the incorrect handling of non-numeric route parameters.  Specifically, the example shows how failing to properly handle non-numeric user IDs can lead to unexpected behavior or application crashes. The solution provides best practices for robust parameter validation and error handling.

## Bug
The bug lies in the `users` route, which attempts to parse a user ID from the request parameter.  If this parameter is not a valid number, the comparison in `users.find` will not return the expected result, potentially leading to an error.