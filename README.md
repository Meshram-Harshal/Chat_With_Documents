# Chat With Documents

Chat With Documents is an interactive document-based chat application that utilizes the LLama model to allow users to upload documents and engage in conversations to retrieve specific information. This project is built to support a variety of document types such as CSV, PDF, and Excel, making it ideal for AI-driven document retrieval and knowledge extraction tasks.

## Project Structure

```
Chat_With_Documents/
├── .chainlit/              # Chainlit configurations
├── __pycache__/            # Cached files for faster execution
├── cache/                  # Caching for model and document data
├── exports/charts/         # Directory for exported chart visualizations
├── .env.example            # Example environment configuration
├── CSV_SAMPLE.csv          # Sample CSV file for testing
├── Medical_Dataset.xlsx    # Sample Excel dataset
├── PDF_SAMPLE.pdf          # Sample PDF file for testing
├── chainlit.md             # Chainlit documentation
├── pandasai.log            # Log file for pandasai operations
├── pic.jpg                 # Sample image
├── requirements.txt        # List of Python dependencies
└── streamlit_app.py        # Main Streamlit application
```

## Features

- **Document Upload**: Supports CSV, PDF, and Excel files for flexible document interactions.
- **Natural Language Interaction**: Users can query documents in natural language, supported by the LLama model.
- **Data Visualization**: Generates charts and visualizations based on data queries.
- **Cache Management**: Utilizes caching for faster data retrieval on subsequent queries.
- **Website Chat Support**: Integrates with Chainlit for interactive chat experiences on the web.

## Getting Started

### Prerequisites

- **Python 3.8+**
- **Streamlit**: Required for running the web application.
- **LLama Model**: Ensure LLama model files are set up correctly in your environment.

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/BhojrajCSE21/Chat_With_Documents.git
   cd Chat_With_Documents
   ```

2. Install the required packages:
   ```bash
   pip install -r requirements.txt
   ```

3. Set up your environment variables:
   - Rename `.env.example` to `.env` and update the necessary fields.

### Usage

1. **Run the Application**:
   ```bash
   streamlit run streamlit_app.py
   ```

2. **Upload Documents**: Once the application is running, upload any CSV, PDF, or Excel file to start querying.

3. **Query Documents**: Type your questions or instructions to retrieve information or visualize data from the uploaded document.

## Configuration

- **Environment Variables**: Update `.env` to configure API keys or model parameters.
- **Website Chat Support**: This project includes chat support via Chainlit, which enables website integration for document-based Q&A. Configure Chainlit settings in the `.chainlit/` directory to enable chat interactions on the web.
- **Supported Document Types**: CSV, PDF, and Excel files are supported by default. To add more, modify the `streamlit_app.py` logic.

## Future Enhancements

- **Additional Document Types**: Expand to support DOCX and other formats.
- **Improved Caching**: Implement advanced caching mechanisms to handle large datasets efficiently.

