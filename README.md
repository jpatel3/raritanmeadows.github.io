# Raritan Meadows HOA Website

This is the official website for the Raritan Meadows Homeowners Association in Flemington, New Jersey.

## Local Development

To run the website locally:

1. Make sure you have Python installed on your computer
2. Open a terminal in the project directory
3. Run the following command:
   ```bash
   python serve.py
   ```
4. The website will automatically open in your default web browser
5. To stop the server, press Ctrl+C in the terminal

Alternatively, you can use any other local server of your choice, such as:
- Python's built-in server: `python -m http.server 8000`
- Node.js's `http-server`: `npx http-server`
- PHP's built-in server: `php -S localhost:8000`

## Setup Instructions

### GitHub Pages Setup

1. Create a new GitHub repository named `raritanmeadows.github.io`
2. Push this code to the repository
3. Go to repository Settings > Pages
4. Under "Source", select "main" branch
5. Click "Save"

### Domain Configuration

1. In your domain registrar (where you purchased raritanmeadows.org):
   - Add these DNS records:
     ```
     Type: A
     Name: @
     Value: 185.199.108.153
     Value: 185.199.109.153
     Value: 185.199.110.153
     Value: 185.199.111.153
     ```
   - Add this CNAME record:
     ```
     Type: CNAME
     Name: www
     Value: raritanmeadows.github.io
     ```

2. In your GitHub repository:
   - Go to Settings > Pages
   - Under "Custom domain", enter `raritanmeadows.org`
   - Check "Enforce HTTPS"

## Updating the Website

To update the website:
1. Edit the `index.html` file
2. Commit and push changes to the main branch
3. GitHub Pages will automatically update the website

## Contact

For any questions or issues, please contact the board at board@raritanmeadows.org 