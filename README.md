## Agro Web App

Agro Web App is a web application designed to provide farmers and users with information about crops, government schemes, and to allow users to apply for various agricultural schemes. The app offers both user and admin functionalities, enabling users to view and apply for schemes while allowing admins to post new crop details and schemes.

## Table of Contents

- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Technologies Used](#technologies-used)
- [Contributing](#contributing)
- [License](#license)

## Features

- User registration and login
- Admin dashboard for posting crop details and government schemes
- User dashboard for viewing crop details and government schemes
- Application for government schemes
- Viewing application status
- Firebase authentication and Firestore for data storage

## Installation

To run this project locally, follow these steps:

1. Clone the repository:
    ```sh
    git clone https://github.com/yourusername/agro-web-app.git
    ```

2. Navigate to the project directory:
    ```sh
    cd agro-web-app
    ```

3. Open `index.html` in your preferred browser.

## Usage

### Firebase Configuration

1. Create a Firebase project on the [Firebase Console](https://console.firebase.google.com/).
2. Add a new web app to your project and copy the Firebase configuration.
3. Replace the Firebase configuration in `script.js` with your own configuration:
    ```javascript
    const firebaseConfig = {
        apiKey: "YOUR_API_KEY",
        authDomain: "YOUR_AUTH_DOMAIN",
        projectId: "YOUR_PROJECT_ID",
        storageBucket: "YOUR_STORAGE_BUCKET",
        messagingSenderId: "YOUR_MESSAGING_SENDER_ID",
        appId: "YOUR_APP_ID",
        measurementId: "YOUR_MEASUREMENT_ID"
    };
    firebase.initializeApp(firebaseConfig);

    const auth = firebase.auth();
    const db = firebase.firestore();
    ```

### Running the App

1. Open `index.html` in your browser.
2. Register a new user or login with existing credentials.
3. If logged in as admin (check for a specific email in the script), the admin dashboard will be shown.
4. Users can view crop details, view government schemes, apply for schemes, and check their application status.

## File Structure
agro-web-app/
│
├── index.html # Main HTML file
├── styles.css # CSS file for styling
├── script.js # JavaScript file for functionality
└── README.md # Project documentation

## Technologies Used

- HTML5
- CSS3
- JavaScript
- Firebase Authentication
- Firebase Firestore

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request for any improvements or bug fixes.

1. Fork the repository.
2. Create your feature branch (`git checkout -b feature/AmazingFeature`).
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`).
4. Push to the branch (`git push origin feature/AmazingFeature`).
5. Open a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
MIT License

Copyright (c) [2024] [Chakshu Gupta]

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.