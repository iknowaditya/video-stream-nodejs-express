# Express.js Video Streaming and Upload

This is a simple Express.js project that enables video streaming and upload.

Installation

To run this project, please follow these steps:

Clone this repository on your local machine.
Navigate to the project directory and run npm install to install the required dependencies.
Run npm start to start the server.
Open your browser and go to http://localhost:3000/ to view the HTML file.
How it Works

When the server is started, it listens for requests on port 3000. When a request is made to the root route (/), the index.html file is served to the client. The HTML file contains a video player that plays the video with the path /video.

When a request is made to the /video route, the server reads the video file (video.mp4), calculates the size of the video, and determines the range of bytes to be sent to the client based on the Range header of the request. The server then sends the specified range of bytes to the client with the appropriate Content-Range, Accept-Ranges, Content-Length, and Content-Type headers.

License

This project is licensed under the MIT License. See the LICENSE file for more information.