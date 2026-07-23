# Healthy City Self-Assessment

A Persian-language interactive web application for evaluating a city against Healthy City indicators.

The assessment covers 9 domains and 80 indicators, calculates results automatically, stores progress in the browser, and includes province-level visual feedback.

## Features

- 9 assessment domains and 80 indicators
- Persian right-to-left interface
- Automatic scoring and progress tracking
- Browser-based progress persistence
- Jalali date support
- Printable results
- Responsive desktop and mobile layout
- Province-level visual scoring guide
- Google Sheets submission integration
- Single-file frontend

## Technology

- HTML5
- CSS3
- Vanilla JavaScript
- Google Apps Script / Google Sheets integration
- Vazirmatn font

## Run Locally

```bash
git clone https://github.com/siavashtnejad-ux/HealthyCity.git
cd HealthyCity
python3 -m http.server 8000
```

Open `http://localhost:8000`.

## Google Sheets Integration

The frontend can send assessment information to a Google Apps Script web-app endpoint. Before production use:

1. create a destination Google Sheet;
2. deploy a Google Apps Script web app that validates and stores submissions;
3. place the deployment URL in the frontend configuration;
4. restrict access and validate all incoming fields;
5. test success and failure handling.

Do not place private credentials in `index.html`.

## Data & Privacy

Assessment progress may be stored locally in the browser. If Google Sheets submission is enabled, disclose what data is collected and obtain any necessary consent.

## Author

[Siavash Torkamannejad](https://github.com/siavashtnejad-ux)
