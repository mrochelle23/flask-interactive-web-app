# Flask Fun App

This Flask application provides a fun and interactive platform with various features including animal facts, compliments, image filtering, and GIF searching. Users can engage with the application to receive random compliments, learn interesting facts about animals, filter images, and search for GIFs based on their queries.

## Features

- **Animal Facts**: Users can select an animal and receive a fun fact about it.
- **Compliments**: Users can enter their name and request a specified number of compliments.
- **Image Filtering**: Users can upload an image and apply various filters to it.
- **GIF Search**: Users can search for GIFs based on a query and specify how many GIFs they want to see.

## Technologies Used

- Flask
- HTML/CSS
- Python
- Jinja2 templating engine
- Various third-party APIs (for GIF search)

## Installation

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/yourusername/your-repository.git
   cd your-repository
   ```

2. **Set Up a Virtual Environment** (optional but recommended):
   ```bash
   python3 -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

3. **Install Requirements**:
   ```bash
   pip install -r requirements.txt
   ```

4. **Environment Variables**:
   - Create a `.env` file in the root directory of the project and add your API keys (e.g., for GIF search):
     ```
     API_KEY=your_api_key_here
     ```

## Usage

1. **Run the Application**:
   ```bash
   flask run
   ```

2. **Access the App**:
   Open your web browser and go to `http://127.0.0.1:5000/` to access the home page. From there, you can navigate to different features.

## Testing

To run the tests for the application, use the following command:
```bash
pytest test_app.py
```
