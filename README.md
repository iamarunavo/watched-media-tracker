# Watched Media Tracker

Submitted by: **Carlo Ace Sagad, Jose Huertero, Arunavo Chowdhury**

## Description and Purpose

Watched Media Tracker helps users keep track of the TV shows, anime, movies, and specific seasons/episodes they have watched across various platforms like Netflix, Crunchyroll, etc. The purpose is to provide a centralized place to manage viewing history and easily see what to watch next or where the user left off in a series.

## Inspiration

We often lose track of which season or episode we last watched, especially for ongoing series or anime with many installments. Existing apps can sometimes be overly complex, focused on only one type of media, or lack the specific tracking features we want. We were inspired to create a simple, focused, and visually appealing tool to solve this common problem for ourselves and others who consume a lot of media.

## Feature List

Below is a list of the features we plan to implement for the final project.

**Baseline Features:**

1.  **View Tracked Shows:** Users can view a list/grid of all the shows, anime, or movies they have added to their tracking list. (GET all user's tracked items)
2.  **Add New Show:** Users can add a new show/movie to their tracked list (initially perhaps via manual entry, potentially later via external API search). (POST a new tracked item relationship)
3.  **View Show Details:** Users can click on a show to see more details, including a description, cover image, and a list of its seasons/episodes. (GET show by ID, Frontend Route)
4.  **Mark as Watched/Unwatched:** Users can mark individual seasons or episodes as watched or unwatched. The interface updates instantly. (PATCH/POST on `user_watched_status`, Frontend Interaction)
5.  **Remove Show:** Users can remove a show entirely from their tracked list. (DELETE a tracked item relationship)
6.  **Database Relationships:** Implement database schema with Users, Shows, Seasons/Episodes, and a `user_watched_status` join table representing the many-to-many relationship.
7.  **Database Reset Script:** Include a script to reset the database tables to their initial state.
8.  **RESTful API:** Backend API follows REST principles with appropriate naming conventions for routes.
9.  **React Frontend:** Use React with React Router for frontend navigation and component hierarchy.
10. **Deployment:** Deploy the final application to Render.

**Custom Features:**

1.  **Filter Tracked List:** Users can filter their tracked list by platform (e.g., Netflix, Crunchyroll) or genre. (Custom Feature #1 - Filter/Sort)
2.  **Track Watched Date:** The `user_watched_status` join table will include a `watched_date` column, recording when the user marked an item as watched. (Custom Feature #2 - Unique Field in Join Table)

**Stretch Features (Potential Ideas):**

- Integrate with an external API (like TMDB or TVMaze) to automatically fetch show details and episode lists.
- Implement user authentication (e.g., GitHub OAuth).
- Add a user rating system for watched shows/episodes.
- Display progress bars for partially watched seasons.

_(Note: Add/remove/modify features as your group finalizes the plan)_
