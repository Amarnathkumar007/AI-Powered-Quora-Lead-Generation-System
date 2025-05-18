# AI Powered Quora Lead Generation System

A Streamlit application that helps generate leads from Quora by searching for relevant posts and extracting user information.

## Features

- Searches Quora for relevant posts based on your company description
- Extracts user information including:
  - Username
  - Bio
  - Post type (question/answer)
  - Timestamp
  - Upvotes
  - Links included in posts
- Formats and writes extracted data to Google Sheets

## Requirements

- Python 3.x
- Streamlit
- Firecrawl API key
- OpenAI API key
- Composio API key

## Installation

1. Clone the repository
2. Install required packages:
   ```
   pip install streamlit requests phi firecrawl pydantic composio_phidata
   ```

## Usage

1. Run the application:
   ```
   streamlit run app.py
   ```
2. Enter your API keys in the sidebar:
   - Firecrawl API key
   - OpenAI API key
   - Composio API key
3. Specify the number of links to search (1-10)
4. Describe what kind of leads you're looking for in the text area
5. Click "Generate Leads" button

The application will:
1. Transform your query into a focused search term
2. Search Quora for relevant posts
3. Extract user information from found posts
4. Format the data and write it to a new Google Sheet
5. Provide a link to the generated Google Sheet

## API Key Requirements

- Firecrawl API key from [Firecrawl's website](https://www.firecrawl.dev/app/api-keys)
- OpenAI API key from [OpenAI's website](https://platform.openai.com/api-keys)
- Composio API key from [Composio's website](https://composio.ai)
```
