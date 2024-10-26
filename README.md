```markdown
# Quillbot Proxy Application

This project is a Flask web application that acts as a proxy for the Quillbot paraphrasing service. It allows users to access the functionality of Quillbot, including text paraphrasing, through a simplified interface while managing cookies and session handling.

## Features

- **Homepage Access**: Users can visit the main page of Quillbot through the application.
- **Paraphrasing Service**: Users can submit text to be paraphrased and receive the modified text in response.
- **Proxy Support**: The application can act as a proxy for other Quillbot endpoints, forwarding requests and responses while preserving cookies and session information.

## Technologies Used

- **Flask**: A lightweight web framework for Python used to create the web application.
- **DrissionPage**: A library for browser automation that facilitates interaction with web pages.
- **Requests**: A Python library for making HTTP requests, used to forward requests and manage sessions.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/quillbot-proxy.git
   cd quillbot-proxy
   ```

2. Install the required packages:
   ```bash
   pip install Flask DrissionPage requests
   ```

3. Run the application:
   ```bash
   python app.py
   ```

4. Open your web browser and navigate to `http://localhost:5000` to access the application.

## Usage

- **Homepage**: The main page displays the Quillbot interface, allowing users to access its features directly.
- **Paraphrasing**: Send a POST request to `/paraphrase` with a form parameter `text` containing the text to be paraphrased. The response will contain the paraphrased text.
  
  Example of a POST request using curl:
  ```bash
  curl -X POST -d "text=Your text here" http://localhost:5000/paraphrase
  ```

- **Proxying Other Endpoints**: You can access other Quillbot functionalities by making GET or POST requests to the respective endpoints via the application.

## Cookies

The application utilizes a set of predefined cookies to manage sessions and maintain user login status with Quillbot. Ensure that the cookie values are kept up to date to maintain functionality.

## Notes

- The application may experience downtime if the Quillbot website changes its structure or requires additional authentication measures.
- This project is intended for personal use and educational purposes.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Author

- [Adylbek](https://github.com/yourusername)
```
