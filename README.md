// Import the required modules
const express = require('express');

// Check if Express is installed
try {
    require.resolve('express');
} catch (e) {
    console.error('Express module is not installed. Run "npm install express" before running this script.');
    process.exit(1);
}

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

