# **API Authentication Demonstration**

A practical project that demonstrates how to integrate and utilize different types of authentication methods (No Auth, Basic Auth, API Key, and Bearer Token) with an external API. This project includes a user-friendly front-end interface and a Node.js backend to showcase the interaction.

---

## **Features**
- **Multiple Authentication Methods**:
  - **No Authentication**: Access public endpoints without credentials.
  - **Basic Authentication**: Username and password-based authentication.
  - **API Key**: Secure requests by including an API key as a query parameter.
  - **Bearer Token**: Use a token in the authorization header for secure access.
- **Dynamic API Interaction**:
  - Allows users to test different authentication methods by interacting with the API endpoints.
- **Response Display**:
  - Real-time display of API responses in the front-end.
- **Simplified Interface**:
  - A clean and intuitive interface with buttons for each authentication type.

---

## **Technologies Used**
- **Node.js**: Server-side runtime environment.
- **Express.js**: Framework for creating the API interaction routes.
- **Axios**: Library for making HTTP requests to the external API.
- **EJS (Embedded JavaScript Templates)**: For rendering dynamic HTML content.
- **CSS**: For styling the user interface.

---

## **Getting Started**

### **Prerequisites**
- **Node.js**: Ensure Node.js is installed on your system.

---

### **Installation**
1. Clone the repository:
   ```bash
   git clone https://github.com/Ayu1404/API-Authentication-Demo.git
   cd API-Authentication-Demo
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Add Authentication Credentials:
   - Replace the placeholders in `server.js` with your own credentials:
     ```javascript
     const yourUsername = "your-username";
     const yourPassword = "your-password";
     const yourAPIKey = "your-api-key";
     const yourBearerToken = "your-bearer-token";
     ```

4. Start the server:
   ```bash
   node server.js
   ```

5. Open your browser and navigate to:
   ```plaintext
   http://localhost:3000
   ```

---

## **How to Use**
1. **Access the App**:
   - Open the web interface at `http://localhost:3000`.
2. **Test Authentication Methods**:
   - Click on the buttons to test various authentication mechanisms:
     - **No Auth**: Sends a request to the `/random` endpoint.
     - **Basic Auth**: Retrieves data from the `/all` endpoint (page 2).
     - **API Key**: Filters secrets with an embarrassment score of 5 or greater via the `/filter` endpoint.
     - **Bearer Token**: Retrieves a secret with ID `42` from the `/secrets/{id}` endpoint.
3. **View API Responses**:
   - Responses from the API are displayed dynamically in the "Response Area."

---

## **Routes**
### **Server Routes**
| HTTP Method | Path         | Description                                 |
|-------------|--------------|---------------------------------------------|
| **GET**     | `/`          | Renders the main page with all buttons.     |
| **GET**     | `/noAuth`    | Fetches a random secret without authentication. |
| **GET**     | `/basicAuth` | Retrieves secrets from page 2 using Basic Auth. |
| **GET**     | `/apiKey`    | Filters secrets with a score of 5+ using an API key. |
| **GET**     | `/bearerToken` | Retrieves a secret with ID `42` using a Bearer Token. |

---

## **File Structure**
### **Backend (server.js)**:
- Integrates with the **Secrets API** using Axios for:
  - No Authentication requests.
  - Basic Authentication with username and password.
  - API Key-based requests with query parameters.
  - Bearer Token-based requests with authorization headers.

### **Front-End (index.ejs)**:
- **Button Interface**:
  - Buttons for each authentication method.
- **Response Display**:
  - Displays JSON responses from the API in real-time.

---

## **Example API Interactions**
1. **No Authentication**:
   - Fetches a random secret from `/random`.
2. **Basic Auth**:
   - Retrieves secrets from `/all` (page 2).
3. **API Key**:
   - Filters secrets based on a score of 5 or greater.
4. **Bearer Token**:
   - Retrieves a specific secret (ID: 42).

---

## **Contributing**
Contributions are welcome! To contribute:
1. Fork this repository.
2. Create a new branch:
   ```bash
   git checkout -b feature/your-feature-name
   ```
3. Commit your changes:
   ```bash
   git commit -m "Add your feature"
   ```
4. Push to your branch:
   ```bash
   git push origin feature/your-feature-name
   ```
5. Open a pull request.

---

## **License**
This project is licensed under the MIT License, allowing you to modify and distribute the project with proper attribution.

---

## **Acknowledgments**
- Special thanks to the **Secrets API** for providing the backend functionality.
- Inspired by the goal of understanding and implementing various authentication mechanisms.
