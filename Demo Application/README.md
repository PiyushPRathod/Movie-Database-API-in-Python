# Demo Application

This application demonstrates how to integrate The Movie Database (TMDB) APIs into a real-world application. 

## Overview

In this demo, we will cover the following:

- **Workflow**
- **API Endpoints in Use**

## Workflow

When we run the application, the first page we see is the **home page**. The home page has two main components using the API endpoints: the navigation bar and flashcards.

- **Flashcards**: By hovering over them, users can see basic details of a movie or a TV show. Clicking "View Details" takes us to the movie or TV show details page.
  
### Navigation Bar

The navigation bar on the left side includes:

- **“MovieTV” or “Home”**: Takes us to the home page.
- **“Movies”**: Directs to the movies page, displaying latest, trending, popular, top-rated, upcoming, and currently playing movies.
- **“TV Shows”**: Takes us to the TV page, showing latest, trending, popular, top-rated, airing today, and on-air TV shows.
- **“People”**: Directs to the persons page, where users can see all popular persons on TMDB.

On the right side of the navigation bar, users can select the object to be searched (movie, TV show, or person), type in their query in the search bar, and click the search button or press enter to go to the results page.

## API Endpoints in Use

We have utilized various API endpoints in the `views.py` file. Here's a summary of how each function uses the endpoints:

- **Index Function** (line 10):
  - Uses the **trending** endpoint (line 11) with `media_type` set to all and `time_window` set to day to display trending movies and TV shows on the home page.

- **Search Function** (line 16):
  - Uses the **search** endpoint (line 22) to take the media type (movie or TV) and query string from the user, returning the search results. The `include_adult=false` parameter filters out adult content.

- **Movies Function** (line 33):
  - Displays the “Movies” page using multiple endpoints, including:
    - Latest movie (line 34)
    - Trending movies (line 35)
    - Popular movies (line 36)
    - Top movies (line 37)
    - Upcoming movies (line 38)
    - Now playing movies (line 39)

- **TV Function** (line 50):
  - Displays the “TV Shows” page using multiple endpoints, including:
    - Latest TV shows (line 51)
    - Trending TV shows (line 52)
    - Popular TV shows (line 53)
    - Top TV shows (line 54)
    - TV shows airing today (line 55)
    - On-air TV shows (line 56)

- **Movie Detail Function** (line 67):
  - Displays details for the selected movie using several endpoints:
    - Primary movie details (line 68)
    - Recommendations (line 69)
    - Credits (line 70)
    - Videos (line 71)

- **TV Detail Function** (line 81):
  - Displays details for the selected TV show using several endpoints:
    - Primary TV details (line 82)
    - Recommendations (line 83)
    - Credits (line 84)
    - Videos (line 85)

- **Season Detail Function** (line 95):
  - Displays details for the requested season of a TV show using the **season** endpoint (line 96) that requires `season_number`.

- **Episode Detail Function** (line 103):
  - Displays details for the requested episode of a TV show using the **episode** endpoint (line 104), which requires both `episode_number` and `season_number`.

- **People Detail Function** (line 110):
  - Displays details for the requested person using the **person** endpoint (line 111) with `person_id` as the required parameter. It also uses the **combined_credits** endpoint.

- **People Function** (line 117):
  - Displays all popular persons on TMDB using the **popular** endpoint (line 118).

**Note**: The following widget only shows the necessary files required to explain The Movie Database APIs.

## Conclusion

This demo application effectively showcases the integration of TMDB APIs, providing users with a rich experience for exploring movies and TV shows. Feel free to explore the code and customize it for your needs!

