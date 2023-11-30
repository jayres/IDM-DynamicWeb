# Exercise Six: Users and Authentication

The purpose of this exercise is to get create users and allow users to authenticate to your site.

## Steps

1. Create a Next.js instance and push it to your Github
2. Create the components you will need (and put in some filler content):

- Components
  - Login Form
  - Create User Form
  - User Profile Components
- Pages
  - Login Page
  - Create User Form
  - User Profile Page

3. Sign up to Vercel and deploy to Vercel
4. Set up routes/pages for your project
5. Create a global wrapper (\_app.js)
6. Create universal header for the project
7. Hook up Firebase to your project and create new Firebase project
8. Setup Firebase Auth (https://firebase.google.com/docs/auth/web/password-auth)
9. Setup Create Account flow
10. Setup Login Flow
11. Setup Logout Flow
12. Display User Profile information on the User Profile page.
13. Display items in header based on user's logged in/out state
14. Send user to login if logged out and user profile if logged in
15. Send a link to your Github repo and a deployed version of the app from Vercel

## Miscellaneous Notes

1. You will have to track whether a user is signed in or not
2. You will have to make sure you are querying data for a user specifically
3. Rely heavily on Firebase for handling the get user and authentication (https://firebase.google.com/docs/auth/web/manage-users#get_a_users_profile)

## Resources

[Firebase Auth](https://firebase.google.com/docs/auth)

[Getting Started with Authentication - Firebase](https://firebase.google.com/docs/auth/web/start)

[Firebase Auth - SDK Web](https://firebase.google.com/docs/auth/web/password-auth)

[Connect Firebase to your Web Project](https://firebase.google.com/docs/web/setup)

[Users in Firebase](https://firebase.google.com/docs/auth/users)

[Managing Users](https://firebase.google.com/docs/auth/web/manage-users#get_the_currently_signed-in_user)

[Auth Persistence](https://firebase.google.com/docs/auth/web/auth-state-persistence)

[Get Currently Signed In User](https://firebase.google.com/docs/auth/web/manage-users#get_the_currently_signed-in_user)

[Single Shared Layout in Next](https://nextjs.org/docs/pages/building-your-application/routing/pages-and-layouts#single-shared-layout-with-custom-app)
