
// Import the required modules
const express = require('express');

// Create an instance of an Express application
const app = express();

// Define a route for the root URL ('/')
app.get('/', (req, res) => {
    res.send('Hello World!');
});

// Start the server and listen on a specific port
const PORT = 3000;
app.listen(PORT, () => {
    console.log(`Server is running on http://localhost:${PORT}`);
});

