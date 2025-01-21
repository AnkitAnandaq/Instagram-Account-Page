# Instagram Account Page Template

This project is a Node.js and Express.js application that renders a dynamic Instagram-like account page using EJS templating engine.

## Features

- **Dynamic Profile Rendering**: Displays user profile data dynamically based on the username in the URL.
- **Stats Section**: Shows total posts, followers, and following count.
- **Gallery**: Dynamically displays posts with images, likes, comments, and captions.
- **Responsive Design**: Ensures usability across various devices.

## Folder Structure

```
project-root/
├── views/               # EJS templates for rendering the pages
│   ├── index.ejs        # Main template for the Instagram page
├── data.json            # JSON file containing user data
├── index.js             # Main server file
├── package.json         # Project dependencies
├── node_modules/        # Installed dependencies
├── public/              # Static files (if added)
├── README.md            # Project documentation
```

## Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/Instagram-Account-Page.git
   ```
2. Navigate to the project directory:
   ```bash
   cd Instagram-Account-Page
   ```
3. Install dependencies:
   ```bash
   npm install
   ```
4. Start the server:
   ```bash
   node index.js
   ```
5. Open your browser and visit:
   ```
   http://localhost:8000/instagram/:username
   ```
   Replace `:username` with a valid username from `data.json`.

## Technologies Used

- **Node.js**: Server-side runtime environment.
- **Express.js**: Web framework for building the server.
- **EJS**: Embedded JavaScript templating for rendering dynamic views.
- **HTML & CSS**: For the front-end design.

## Example `data.json` Structure

```json
{
  "johndoe": {
    "name": "John Doe",
    "bio": "Photographer & Traveler",
    "followers": 1234,
    "following": 567,
    "posts": [
      {
        "image": "images/post1.jpg",
        "likes": 345,
        "comments": ["Awesome!", "Great shot!"],
        "caption": "Beautiful sunset at the beach."
      },
      {
        "image": "images/post2.jpg",
        "likes": 290,
        "comments": ["Lovely view!"],
        "caption": "Exploring the mountains."
      }
    ]
  }
}
```

## Future Enhancements

- Add a database to store user data.
- Implement user authentication.
- Add client-side interactivity with JavaScript.

## License

This project is licensed under the MIT License. Feel free to use and modify it as needed.

## Contributing

Contributions are welcome! If you have suggestions or improvements, feel free to submit a pull request.
