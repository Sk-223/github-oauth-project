# OAuth 2.0 Project
## Overview
This project demonstrates the implementation of OAuth 2.0 for user authentication and authorization. It is part of the Codecademy Full-Stack Engineer path, specifically focusing on back-end development.

## Table of Contents
- [Features](#features)
- [Implementation Details](#implementation-details)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)
- [Contributions](#contributions)
- [License](#license)
- [Acknowledgements](#acknowledgements)
- [Contact](#contact)

## Features
- User authentication using OAuth 2.0
- Secure access to protected resources
- Integration with third-party OAuth providers

## Implementation Details
### OAuth 2.0 Flow
1. **Authorization Request**: The user is redirected to the OAuth provider's authorization server.
2. **User Authorization**: The user logs in and grants permission to the application.
3. **Authorization Code**: The authorization server redirects the user back to the application with an authorization code.
4. **Access Token Request**: The application exchanges the authorization code for an access token.
5. **Access Token Response**: The authorization server returns the access token.
6. **Access Protected Resources**: The application uses the access token to access protected resources on behalf of the user.

## Technologies Used
- **Node.js**: Server-side JavaScript runtime.
- **Express**: Web framework for Node.js.
- **Passport.js**: Authentication middleware for Node.js.
- **OAuth 2.0**: Protocol for authorization.

## Installation

1. **Register OAuth Application on GitHub:**
   - Navigate to GitHub "Settings" > "Developer settings" > "OAuth Apps".
   - Click "Register a new application" and fill out the form:
     - **Application Name:** OAuth Project
     - **Homepage URL:** `http://localhost:3000`
     - **Authorization Callback URL:** `http://localhost:3000/auth/github/callback`
   - Take note of the Client ID and generate a Client Secret. Save these securely.

2. Clone the repository:
    ```bash
    git clone https://github.com/Sk-223/github-oauth-project.git
    cd github-oauth-project
    ```

3. Install dependencies:
    ```bash
    npm install
    ```

4. Set up environment variables:
    Create a `.env` file in the root directory and add your OAuth provider credentials:
    ```env
    CLIENT_ID=your-client-id
    CLIENT_SECRET=your-client-secret
    REDIRECT_URI=http://localhost:3000/auth/callback
    ```

5. Start the application:
    ```bash
    node app.js
    ```

## Usage
1. Open your browser and navigate to `http://localhost:3000`.
2. Click on the "Login" button.
3. Authorize the application to access your account.
4. You will be redirected back to the application with access to protected resources.

## Contributing
Contributions are welcome! Please fork the repository and create a pull request with your changes.

## License
This project is licensed under the MIT License

 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## Acknowledgements
- Codecademy for providing the project framework and resources.
- OAuth 2.0 for the authentication protocol.

## Contact
If you have any questions or feedback, feel free to reach out to me [here](sharonannemccane@gmail.com)!

