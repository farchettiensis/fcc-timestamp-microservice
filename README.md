# Timestamp Microservice

A simple Express.js web service that provides timestamp information for a given date. This is a challenge from the freeCodeCamp's Back End Development and APIs certification. It contains my solution to the challenge.

## Features

- Converts a provided date into Unix timestamp and UTC format.
- Handles various date formats, including Unix timestamps.
- Provides a current timestamp if no date is specified.
- Returns an error message for invalid date parameters.

### Usage

1. Start the server:

   ```bash
   npm start
   ```

2. Open the browser and go to [http://localhost:3000](http://localhost:3000).

3. Use the following endpoints to get timestamp information:

   - `/api/:date?`: Returns a JSON object with Unix timestamp and UTC time for the provided date.

   Example:

   ```bash
   http://localhost:3000/api/2024-01-26
   ```

   Response:

   ```json
   {
     "unix": 1674748800000,
     "utc": "Wed, 26 Jan 2024 00:00:00 GMT"
   }
   ```

   If no date is provided, the current timestamp is returned.

4. To stop the server, press `Ctrl + C` in the terminal.

## Built With

- [Node.js](https://nodejs.org/)
- [Express.js](https://expressjs.com/)