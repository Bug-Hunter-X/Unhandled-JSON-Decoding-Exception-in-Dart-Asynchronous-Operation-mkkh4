# Unhandled JSON Decoding Exception in Dart

This repository showcases a common error in Dart asynchronous programming related to JSON decoding and its solution. The `bug.dart` file contains code that uses `jsonDecode` without properly handling potential `FormatException` exceptions that can occur if the JSON response is invalid or malformed.  The solution in `bugSolution.dart` addresses this issue.

The problem is that a `FormatException` might occur during `jsonDecode` if the API returns malformed or unexpected JSON, causing the program to crash without a clear indication of the error. The improved code adds a `try-catch` block specifically for this case, enabling more robust error handling. This makes the application more resilient and provides better feedback to the user.