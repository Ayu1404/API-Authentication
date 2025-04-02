
# **API Authentication**

A comprehensive project demonstrating various types of authentication in web development, implemented using Express.js. This project showcases secure practices for handling credentials and making API calls using `No Auth`, `Basic Auth`, `API Key`, and `Bearer Token`.


## **Features**
- **No Authentication**: Fetch data from the API without any authentication.
- **Basic Authentication**: Securely access the API using a username and password.
- **API Key Authentication**: Use an API key to filter and retrieve specific data.
- **Bearer Token Authentication**: Fetch restricted data using an authorization token.
- **Environment Variables**: Manage sensitive credentials using `.env` files.


## **Getting Started**

Follow these steps to set up and run the project locally:

### **Prerequisites**
Ensure you have the following installed on your system:
- Node.js
- npm (Node Package Manager)

### **Installation**
1. Clone the repository:
   ```bash
   git clone https://github.com/Ayu1404/ExpressAuthDemo.git
   cd ExpressAuthDemo
   ```
2. Install dependencies:
   ```bash
   npm install
   ```

3. Create a `.env` file in the root directory to securely store authentication credentials:
   ```env
   API_USERNAME=your_username
   API_PASSWORD=your_password
   API_KEY=your_api_key
   BEARER_TOKEN=your_bearer_token
   ```

4. Start the server:
   ```bash
   npm start
   ```


## **Usage**
1. Access the application by navigating to `http://localhost:3000` in your browser.
2. Click buttons on the interface to make API requests:
   - **No Auth**: Fetch random secrets.
   - **Basic Auth**: Fetch secrets with authentication.
   - **API Key**: Filter secrets by score using an API key.
   - **Bearer Token**: Retrieve specific secrets using a bearer token.



## **Technologies Used**
- **Backend**: Node.js, Express.js, Axios
- **Frontend**: HTML, CSS
- **Environment Management**: dotenv



## **Key Concepts**
1. **Environment Variables**:
   - Securely store sensitive credentials (username, password, API key, bearer token) in a `.env` file.
   - Keep them out of your source code.

2. **Authentication Types**:
   - **Basic Authentication**: Use a username and password for accessing restricted API endpoints.
   - **API Key**: Query parameters help authenticate requests.
   - **Bearer Token**: Use authorization headers to secure API calls.

3. **Error Handling**:
   - Handles API response errors gracefully (e.g., 401 Unauthorized, 404 Not Found).



## **Contributing**
Contributions are welcome to improve functionality or add new features. Here's how to contribute:
1. Fork the repository.
2. Create a new branch for your feature:
   ```bash
   git checkout -b feature/new-feature
   ```
3. Commit your changes and push the branch:
   ```bash
   git push origin feature/new-feature
   ```
4. Open a pull request and describe the changes you’ve made.

---

## **License**
This project is licensed under the MIT License. Feel free to use, modify, and distribute it.

---

## **Acknowledgments**
- Special thanks to [Secrets API](https://secrets-api.appbrewery.com) for providing the endpoints.
- Inspiration drawn from modern authentication practices.
