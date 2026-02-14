# GreenGuard V2 Upgrade Plan

## User Review Required
> [!IMPORTANT]
> This upgrade introduces URL scraping capabilities. Ensure `cheerio` and `axios` are installed in the backend.

## Proposed Changes

### Backend (`server/index.js`)
- **[MODIFY]** Update `/analyze` endpoint to accept `url` and `category` in request body.
- **[NEW]** Implement URL scraping logic using `axios` and `cheerio`.
- **[MODIFY]** Update Mock AI logic to return category-specific results (e.g., Fashion -> polyester/labor issues).
- **[MODIFY]** Update Gemini prompt to include category context.

### Frontend (`client/src`)
#### Components
- **[MODIFY] `AnalyzeForm.jsx`**:
    - Add Tabs for "Text" vs "URL" mode.
    - Add Dropdown for Industry Category selection.
    - Update form submission to send `url` or `text` and `category`.
- **[NEW] `components/SocialFeed.jsx`**:
    - Create a horizontal scrolling list/grid of mock "Recent Scans".
    - Use Red/Yellow/Green color coding.
- **[MODIFY] `App.jsx`**:
    - Import and render `SocialFeed` below the main results area.

## Verification Plan
### Manual Verification
- **Category Test**: Select "Fashion" and input/url -> Verify response mentions fashion-related issues (mock or real).
- **URL Test**: Paste a legitimate URL -> Verify text is scraped and analyzed (or mock URL response triggered).
- **Social Feed**: Verify "Wall of Shame" is visible and scrolls/renders correctly.
