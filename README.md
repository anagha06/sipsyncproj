SipSync
=======

Overview
--------

SipSync is a cafe-matching application built using Xcode/Swift, leveraging NLP and semantic search to rank cafes based on user preferences. Unlike traditional map applications that rank cafes by proximity, SipSync personalizes recommendations by analyzing both numerical and textual inputs, providing a tailored cafe experience.

Features
--------

*   **Personalized Cafe Ranking**: Uses NLP techniques to analyze cafe reviews and compare them with user queries.
    
*   **Custom Filters**: Users can set preferences through sliders, toggles, and text inputs to refine their search.
    
*   **Cafe Visit Tracking**: Users can log past visits and receive tailored future recommendations.
    
*   **Integrated Mapping**: Utilizes Apple MapKit and Google Places API to display and rank nearby cafes.
    

App Walkthrough
---------------

1.  **Login View**: Entry point for the app; currently uses local variables but will integrate with SQL/Flask for user authentication.
    
2.  **Map View**: Displays optimal cafes on an interactive map and list view; allows users to refine preferences.
    
3.  **Preferences View**: UI for filtering algorithm, allowing users to customize their cafe search.
    
4.  **Profile View**: Shows user details, past visits, and previous cafe ratings.
    

Tech Stack & Frameworks
-----------------------

### Frontend

*   Swift, Xcode, NavigationView for app navigation.
    

### Mapping & Data Fetching

*   **Apple MapKit**: Displays cafe locations via placemarks and MapItems.
    
*   **Google Places API**: Retrieves detailed cafe information (ratings, reviews, ambiance, etc.).
    

### Data Handling

*   Initial dataset scraped via Python script for ~100 cafes near Berkeley.
    
*   Merges MapKit and Places API data, filling in missing details where necessary.
    

### Filtering Algorithm

*   Accepts user-defined filters (e.g., ambiance, drink quality, seating availability).
    
*   Processes cafe reviews using NLP techniques to match user preferences.
    
*   Assigns weighted scores to cafes based on both user input and aggregated data.
    
*   Dynamically updates rankings based on user preferences and historical data.
    

Future Steps
------------

*   **Improve Data Integration**: Expand dataset and transition to a real-time API-based solution.
    
*   **User Authentication & Profiles**: Implement SQL/Flask backend for user accounts.
    
*   **Enhanced NLP Matching**: Improve ranking algorithm with more advanced semantic search techniques.
    
*   **Mobile Optimization**: Enhance UI/UX for a smoother and more interactive user experience.
    

### Author

Developed as a capstone project to revolutionize the cafe discovery experience through AI-driven personalization.
