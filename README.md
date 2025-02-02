# Node.js Server Unresponsiveness Bug

This repository demonstrates a common issue in Node.js servers: unresponsiveness caused by long-running operations within the request handler.  The provided `server.js` file contains a simple HTTP server that simulates a long-running task (5-second CPU-bound operation).  During this time, the server cannot accept new requests, leading to timeouts and poor user experience.

The solution, found in `server-solution.js`, demonstrates how to address this issue using asynchronous operations and appropriate task management techniques (e.g., using worker threads, promises, or task queues for CPU-bound operations).