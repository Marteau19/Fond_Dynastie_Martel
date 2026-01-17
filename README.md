# Investment Tracking Dashboard for Léonie & Éliot

A simple, beautiful web page to track and share investment information with your kids.

## Features

- Clean, responsive design that works on all devices
- Easy-to-update JSON data file
- Automatic calculations and formatting
- Beautiful gradient design with card-based layout
- Color-coded returns (green for positive, red for negative)

## How to Update the Data

Simply edit the `data.json` file with your latest values. Here's what each field means:

```json
{
  "fund": {
    "value": 400.00,           // Total value of the fund
    "totalShares": 40,          // Total number of shares
    "sharePrice": 10.00         // Current price per share
  },
  "investors": [
    {
      "name": "Léonie",
      "investment": 180.00,     // Original investment amount
      "shares": 18,             // Number of shares owned
      "currentValue": 180.00,   // Current value (shares × sharePrice)
      "return": 0.00            // Return percentage
    }
  ],
  "performance": {
    "ytd": 0.00,               // Year-to-date performance %
    "oneYear": 0.00,           // 1-year performance %
    "twoYears": 0.00           // 2-year performance %
  }
}
```

## Deploying to GitHub Pages

1. Push this repository to GitHub
2. Go to your repository settings
3. Navigate to "Pages" in the left sidebar
4. Under "Source", select the branch (usually `main` or `master`)
5. Click "Save"
6. Your site will be available at: `https://[your-username].github.io/Fond_Eliot_Leonie/`

## Quick Update Methods

### Method 1: Edit on GitHub (Easiest)
1. Go to your repository on GitHub
2. Click on `data.json`
3. Click the pencil icon (Edit this file)
4. Make your changes
5. Scroll down and click "Commit changes"
6. Your site will update automatically in a few seconds

### Method 2: Edit Locally
1. Clone the repository
2. Edit `data.json` with any text editor
3. Commit and push:
   ```bash
   git add data.json
   git commit -m "Update investment data"
   git push
   ```

### Method 3: From Google Sheets
If you track data in Google Sheets, you can:
1. Update your Google Sheet
2. Copy the values
3. Update `data.json` using Method 1 or 2 above

## Calculating Values

To help you update the data correctly:

- **Current Value** = shares × sharePrice
- **Return %** = ((currentValue - investment) / investment) × 100

## Customization

You can easily customize the appearance by editing `index.html`:
- Colors: Search for `#667eea` and `#764ba2` to change the gradient
- Font: Change the `font-family` in the CSS section
- Add more investors: Just add more objects to the `investors` array in `data.json`

## Files

- `index.html` - The main web page (includes HTML, CSS, and JavaScript)
- `data.json` - The data file you'll update regularly
- `README.md` - This file

## Support

If you need help, feel free to reach out or consult the GitHub Pages documentation.

---

Made with ❤️ for Léonie & Éliot
