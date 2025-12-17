# TradingView Ad Blocker( 2025)

This userscript, combined with uBlock Origin Lite, blocks ads and the "Ad blocker detected" popup on TradingView.com.

## Requirements
- Install these two extensions from the Chrome Web Store:
  - [Tampermonkey](https://chrome.google.com/webstore/detail/tampermonkey/dhdgffkkebhmkfjojejmpbldmpobfkfo)
  - [uBlock Origin Lite](https://chrome.google.com/webstore/detail/ublock-origin-lite/ddkjiahejlhfcafbddmgiahcpfecfmjg)

## Step 1: Install the Tampermonkey Userscript
1. Copy the script code from the main file in this repository.
2. Open the Tampermonkey dashboard (click the extension icon → Dashboard).
3. Click **Create a new script** (or the + tab).
4. Delete the default code.
5. Paste the copied script code.
6. Save it: **File → Save** (or Ctrl+S).

The script will now run automatically on TradingView.com.

## Step 2: Add Custom Filters to uBlock Origin Lite
1. Open uBlock Origin Lite settings (click the extension icon → gear icon).
2. Go to the **My filters** tab.
3. Add these two lines to the text area:

```
tradingview.com##div[class*="dialog"]:has-text(/Ad blocker detected/)
tradingview.com##div:has-text(/Ad blocker detected/)
```

4. Click **Apply changes**.
