# USL Shortened Build Using NodeJs

A URL shortener application built using Node.js. This project allows users to shorten long URLs into concise, easily shareable links. It also provides functionality to manage and analyze shortened URLs.

## Features
- **URL Shortening**: Convert long URLs into short, user-friendly links.
- **Redirection**: Redirect users to the original URL when the short link is accessed.
- **Analytics**: Track usage statistics for shortened URLs, including click counts.
- **API Integration**: Easily integrate with other applications using RESTful APIs.
- **Scalable Design**: Built to handle high traffic and large datasets.

## Steps to Use
1. **Clone the Repository**: 
   ```bash
   git clone <repository-url>
   cd usl-shortened-build
   ```

2. **Install Dependencies**: 
   ```bash
   npm install
   ```

3. **Setup Environment Variables**:
   - Create a `.env` file in the root directory.
   - Add the following variables:
     ```env
     PORT=3000
     MONGO_URI=<your-mongodb-connection-string>
     BASE_URL=<your-base-url>
     ```

4. **Start the Server**: 
   ```bash
   npm start
   ```

5. **Access the Application**:
   - Navigate to `http://localhost:3000` in your web browser.

## Prerequisites
- Node.js (v14 or higher)
- MongoDB instance

## API Endpoints
- **POST /shorten**: Create a shortened URL.
- **GET /:shortCode**: Redirect to the original URL.
- **GET /analytics/:shortCode**: Get analytics for a shortened URL.

## License
This project is licensed under the MIT License. See the LICENSE file for details.
