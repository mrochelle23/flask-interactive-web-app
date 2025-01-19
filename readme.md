# Flask Interactive Web App

This is a simple Flask web application that includes several interactive routes, such as generating compliments, displaying animal facts, applying image filters, and searching for GIFs. It is designed to be a fun and engaging project that demonstrates the use of Flask with several features like user input handling, file uploads, and integration with external APIs.


## Features

1. **Compliments Generator**  
   Generate random compliments for yourself! You can specify how many compliments you want and receive them instantly.

2. **Animal Facts**  
   Select an animal from a list, and get an interesting fact about it. Learn fun and unique facts about animals like koalas, parrots, and mantis shrimp.

3. **Image Filtering**  
   Upload an image and apply various filters (e.g., blur, contour, sharpen) to the image using the Pillow library. The filtered image is displayed after processing.

4. **GIF Search**  
   Search for GIFs using the Tenor API. Enter a search term (e.g., "funny," "cat") and choose how many GIFs to display. The application will return the requested number of GIFs.

## Technologies Used

- Python 3.x
- Flask
- Pillow (for image processing)
- Requests (for making HTTP requests)
- python-dotenv (for managing environment variables)

## Installation

1. Clone this repository to your local machine:

   ```bash
   git clone https://github.com/your-username/flask-web-app.git
   cd flask-web-app
   ```

2. Set up a virtual environment (optional but recommended):

   ```bash
   python3 -m venv venv
   source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
   ```

3. Install the required dependencies:

   ```bash
   pip install -r requirements.txt
   ```

4. Create a `.env` file in the root directory of the project and add your Tenor API key:

   ```
   API_KEY=your_tenor_api_key_here
   ```

   You can get an API key by signing up for an account on [Tenor](https://tenor.com/gifapi).

## Running the Application

1. To start the Flask development server, run:

   ```bash
   python app.py
   ```

2. Navigate to `http://127.0.0.1:5000/` in your web browser to access the app.

## File Structure

```
/your_project_directory
│
├── app.py                  # Flask app file
├── .env                    # Environment file (for API keys and configurations)
├── /templates              # Folder containing HTML templates
│   ├── base.html
│   ├── home.html
│   ├── compliments_form.html
│   ├── compliments_results.html
│   ├── animal_facts.html
│   ├── image_filter.html
│   └── gif_search.html
└── /static                 # Folder containing static files like images, styles.css
    ├── styles.css          # Custom CSS styles
    └── /images             # Filtered images and other uploaded images
```

## Usage

### Homepage

- The homepage provides links to all the app's main features:
  - **Compliments**
  - **Animal Facts**
  - **Image Filter**
  - **GIF Search**

### Compliments

- Input your name, choose whether you'd like compliments, and select how many compliments you'd like to receive (up to 5). The app will generate random compliments for you.

### Animal Facts

- Choose an animal from the list (e.g., koala, lion, mantis shrimp), and get a fun fact about the selected animal.

### Image Filter

- Upload an image and select a filter (e.g., blur, sharpen, emboss). The app will apply the filter to the image and display the result.

### GIF Search

- Enter a search query (e.g., "funny," "cat") and specify the number of GIFs you want. The app will return GIFs from Tenor based on your query.

## Testing

To run the tests for the application, use the following command:
```bash
pytest test_app.py
```
