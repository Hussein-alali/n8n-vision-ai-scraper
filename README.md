# n8n Vision AI Scraper

This workflow automates product data extraction using Google Gemini, ScrapingBee, and Google Sheets.


## Overview
- Takes product URLs from Google Sheets.
- Captures screenshots with ScrapingBee.
- Uses Google Gemini to extract structured data:
  - Product title
  - Price
  - Brand
  - Promo and discount
- Saves clean data back into Google Sheets.

## Tools Used
- ScrapingBee API (for screenshots and HTML)
- Google Gemini (for AI extraction)
- Google Sheets (for input and output)
- n8n (for orchestration)

## How to Run
1. Import `vision-ai-scraper.json` into n8n.
2. Add your API credentials:
   - ScrapingBee API key
   - Google Gemini API
   - Google Sheets connection
3. Update Google Sheet IDs in the workflow.
4. Click “Execute Workflow” or schedule it.

## Output
Results are saved automatically into your target Google Sheet with:
- product_url
- product_title
- product_price
- product_brand
- promo
- promo_percent
