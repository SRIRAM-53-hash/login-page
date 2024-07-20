

# GitHub Repository Documentation

## Project Overview

This project contains a series of HTML pages styled with CSS for a user login and sign-up system. The pages feature a background image with a blur effect for improved readability and visual appeal.

## Project Structure

The project directory structure is as follows:

```
/project-root
    /images
        background.jpg
    index.html
    login.html
    signup.html
    styles.css
```

## Files Description

1. **`index.html`**: Welcome page offering navigation to the login and sign-up pages.
2. **`login.html`**: Login page where registered users can enter their credentials.
3. **`signup.html`**: Sign-up page for new users to create an account.
4. **`styles.css`**: Contains CSS styles for the project. (Optional if you are including inline styles in HTML)

## Setting Up the Project

### 1. **Clone the Repository**

To clone the repository to your local machine, use:

```bash
git clone https://github.com/your-username/your-repo-name.git
```

Replace `your-username` and `your-repo-name` with your GitHub username and repository name.

### 2. **Project Files**

Ensure that the directory structure is as follows:

```
/project-root
    /images
        background.jpg
    index.html
    login.html
    signup.html
    styles.css
```

### 3. **Background Image**

Place your background image in the `images` folder. The image should be named `background.jpg` or adjust the filename in the HTML files accordingly.

## HTML and CSS Setup

### Inline CSS in HTML

To style your pages and apply the background image, use the following inline CSS. Add this CSS code within a `<style>` tag in each HTML file as demonstrated below.

#### Example CSS for `index.html`

```html
<style>
    body {
        font-family: Arial, sans-serif;
        background: url('images/background.jpg') no-repeat center center fixed;
        background-size: cover;
        display: flex;
        justify-content: center;
        align-items: center;
        height: 100vh;
        margin: 0;
        position: relative;
    }
    body::before {
        content: "";
        position: fixed;
        top: 0;
        left: 0;
        height: 100%;
        width: 100%;
        background: inherit;
        filter: blur(8px);
        z-index: -1;
    }
    .welcome-container {
        background-color: rgba(255, 255, 255, 0.9);
        padding: 30px;
        border-radius: 15px;
        box-shadow: 0 0 15px rgba(0, 0, 0, 0.2);
        text-align: center;
        width: 300px;
    }
    h2 {
        margin-bottom: 20px;
        font-size: 24px;
        color: #333;
    }
    p {
        font-size: 18px;
        margin-bottom: 30px;
        color: #666;
    }
    button {
        width: 100%;
        padding: 15px;
        background-color: #007BFF;
        color: white;
        border: none;
        border-radius: 8px;
        font-size: 18px;
        cursor: pointer;
        margin-top: 10px;
        transition: background-color 0.3s;
    }
    button:hover {
        background-color: #0056b3;
    }
    .back-button {
        background-color: #6c757d;
    }
    .back-button:hover {
        background-color: #5a6268;
    }
</style>
```

### HTML Code Examples

Here’s a sample of the HTML code for the **login.html** page with inline CSS.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Login Page</title>
    <style>
        /* Add the inline CSS code here as shown above */
    </style>
</head>
<body>
    <div class="form-container">
        <form action="/login" method="POST">
            <h2>Login</h2>
            <div class="input-group">
                <label for="username">Username</label>
                <input type="text" id="username" name="username" required>
            </div>
            <div class="input-group">
                <label for="password">Password</label>
                <input type="password" id="password" name="password" required>
            </div>
            <button type="submit">Login</button>
            <button type="button" onclick="window.location.href='index.html'" class="back-button">Back</button>
        </form>
    </div>
</body>
</html>
```

## How to Use

1. **Open the `index.html` file** in your browser to view the welcome page.
2. **Navigate to the login or sign-up page** by clicking the respective buttons.
3. **Fill out the forms** on the login and sign-up pages as needed.

## Contributing

If you wish to contribute to this project:

1. **Fork the repository** on GitHub.
2. **Create a new branch** for your changes.
3. **Commit your changes** and push them to your forked repository.
4. **Submit a pull request** to the original repository.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

