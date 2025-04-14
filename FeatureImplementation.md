# Feature Implementation - Buzzly Sponsor Dashboard

## Features I Implemented

### Sponsor Authentication Middleware

- Middleware that checks if a user is logged in as a Sponsor before accessing sponsor-related pages
- If not authenticated → user is redirected to the login page
- Helps protect sponsor-specific routes in the Sponsor Dashboard

---

### Survey Management Feature

- Created Survey Management page for sponsors
- Sponsors can:
  - View all their surveys (GET)
  - Create a new survey (POST)
  - Update an existing survey (PUT)
  - Delete a survey (DELETE)
- API routes handle validation and require the user to be authenticated as a Sponsor
- Data stored and managed in Strapi CMS

---

### Challenge Management Feature

- Created Challenge Management page for sponsors
- Sponsors can:
  - View all their challenges (GET)
  - Create a new challenge (POST)
  - Update an existing challenge (PUT)
  - Delete a challenge (DELETE)
- API routes handle validation and require the user to be authenticated as a Sponsor
- Data stored and managed in Strapi CMS

---

### Sponsor Profile Feature

- Created Sponsor Profile page for sponsors to view their profile information
- Sponsors can:
  - View their own profile details (GET)
- API route requires the user to be authenticated as a Sponsor
- Data is pulled from Strapi CMS
- Displays sponsor-specific details like name, email, company, and logo

---

## Notes for Developers

- All API routes live in `/api/sponsor/`
- Auth is handled using Bearer Tokens provided by Strapi
- Each sponsor can only access and manage their own surveys, challenges, and profile
- Errors and validations return clear messages for frontend handling

---

## GitHub Repo

https://github.com/buzzly-nz/buzzly-next-app
