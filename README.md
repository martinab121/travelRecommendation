# TravelBloom - Travel Recommendation Website

A static multi-page travel website built with HTML, CSS and vanilla JavaScript. Visitors can search by keyword to get destination recommendations for beaches, temples or countries.

## Features

- Home page with navigation bar, introduction section and social media links
- Keyword search for `beach` / `beaches`, `temple` / `temples` and `country` / `countries` (case-insensitive)
- Results shown as cards with an image, name and description; country results also list their cities
- "No results found" message for unmatched keywords and a Reset button to clear results
- About Us page with a team section
- Contact Us page with a name / email / message form (front end only, no backend is included)

## Tech stack

| Area | Technology |
| --- | --- |
| Markup | HTML5 |
| Styling | CSS3, Font Awesome icons (CDN) |
| Logic | Vanilla JavaScript (DOM manipulation, Fetch API) |
| Data | JSON (`travel_recommendation_api.json`) |

## Project structure

```
travel_recommendation.html      # Home page with search
about_us.html                   # About Us page
contact_us.html                 # Contact Us page
travel_recommendation.css       # Shared styles
travel_recommendation.js        # Search and results logic
travel_recommendation_api.json  # Destination data (countries, temples, beaches)
```

The search results are built from destination data defined in `travel_recommendation.js`, which mirrors the contents of `travel_recommendation_api.json`.

## Getting started

No build step or dependencies are required. Open `travel_recommendation.html` in a browser.

To let the page load the JSON file with `fetch`, serve the folder over HTTP instead, for example:

```bash
python3 -m http.server 8000
```

and open `http://localhost:8000/travel_recommendation.html`.

---

Learning project.
