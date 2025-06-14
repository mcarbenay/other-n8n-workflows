# Vision-Based AI Agent Scraper - with Google Sheets, ScrapingBee, and Gemini

## Description
This workflow enables vision-based web scraping using ScrapingBee and integrates with Google Sheets and Gemini for structured data processing.

## Nodes
1. **Manual Trigger**: Initiates the workflow manually.
2. **ScrapingBee - Get page HTML**: Fetches the HTML content of a webpage using ScrapingBee.
3. **Structured Output Parser**: Parses the structured output from the scraped data.
4. **Google Gemini Chat Model**: Processes data using the Google Gemini AI model.
5. **Split Out**: Splits the output into individual items.
6. **Google Sheets - Get list of URLs**: Retrieves a list of URLs from Google Sheets.

## Web Services Involved
- **ScrapingBee**: Used for web scraping.
- **Google Sheets**: Used for data storage and retrieval.
- **Google Gemini**: Used for AI processing.
