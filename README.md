## React Native Data Fetching Bug

This repository demonstrates a common issue encountered when fetching data in React Native applications.  The `DataFetch.js` file contains code that attempts to fetch data from a JSONPlaceholder API endpoint.  Under certain network conditions or API issues, this code can result in an unexpected error or crash. The `DataFetchSolution.js` shows the corrected code.

**Problem:** The original code lacks robust error handling.  Network requests can fail for various reasons (timeout, server error, etc.), and the application may not handle these failures gracefully, leading to crashes or unhelpful error messages to the user.

**Solution:** The corrected version includes more comprehensive error handling, using try...catch blocks to catch potential errors during the fetch process. It also includes a user-friendly error message in case of failure.  The loading state provides feedback to the user while fetching.