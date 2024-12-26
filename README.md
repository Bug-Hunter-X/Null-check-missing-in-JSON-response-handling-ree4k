# Dart JSON Null Check Bug

This repository demonstrates a common error in Dart when handling JSON responses from network requests and provides a solution.

The bug is in `bug.dart`. The code doesn't handle the case where the JSON response might not contain the expected keys. Accessing nested properties like `jsonData['user']['name']` without checking for null values can lead to runtime errors.

The solution (`bugSolution.dart`) shows how to properly check for null values before accessing nested properties, making the code more robust.

## How to run

1. Clone this repository.
2. Run `bug.dart` to see the error.
3. Run `bugSolution.dart` to see the corrected code.