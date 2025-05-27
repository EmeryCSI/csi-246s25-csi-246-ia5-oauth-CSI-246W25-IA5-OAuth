# Renton Technical College CSI-246

<div align="center">  
  <img src="logo.jpg" alt="Logo">
  <h3 align="center">Independent Activity 4: OAuth with Multiple Providers</h3>
</div>

## Overview

In this assignment, you will create a Next.js application which uses OAuth authentication from **two** providers other than Google (e.g., GitHub, Facebook, Twitter, etc.). You will use NextAuth to handle the OAuth flow for these providers and build a basic UI that supports signin and signout. In addition, you will create:

- A navigation bar that displays signin/signout options.
- At least one protected client page.
- At least one protected server page.
- One protected API route.

This activity will help you understand the configuration differences between OAuth providers, how to secure both client and server routes, and how to integrate NextAuth into a full-stack Next.js application.

---

## Requirements

1. **OAuth Providers**
   - Choose any two OAuth Providers. For example:
     - **Google**
     - **GitHub**
     - **Discord**
     - **Twitch**
     - https://next-auth.js.org/providers/
   - Configure each provider using NextAuth. Make sure you follow the provider-specific documentation for obtaining client credentials:
     - For GitHub, refer to [GitHub OAuth documentation](https://docs.github.com/en/developers/apps/authorizing-oauth-apps).
     - For Facebook, refer to [Facebook Login documentation](https://developers.facebook.com/docs/facebook-login/).

2. **Authentication Functionality**
   - Implement signin and signout functionality for both providers using NextAuth.
   - Ensure that your OAuth callback URIs are correctly set (e.g., `http://localhost:3000/api/auth/callback/github` for GitHub).

3. **User Interface**
   - **Navigation Bar:**  
     Create a navbar that shows a "Login" button when the user is not authenticated and a "Logout" button (along with the user’s email or name) when the user is authenticated.
   - **Protected Client Page:**  
     Create at least one page that is protected behind authorization on the client side.
   - **Protected Server Page:**  
     Create at least one server-rendered page that is protected behind authorization on the.
   - **Protected API Route:**  
     Create one API route that is protected. Requests to this API should only be processed if the user is authenticated.

## Submission

1. **Ensure all features are working:**
   - Two OAuth providers (other than Google) are configured.
   - Signin and signout functionality is operational.
   - A navigation bar displays signin/signout options correctly.
   - There is at least one protected client page, one protected server page, and one protected API route.

2. **Commit your changes:**

   ```bash
   git add .
   git commit -m "Independent Activity 4 Complete"
   git push
   ```

3. **Verify:**  
   Your repository should include:
   - NextAuth configuration with two non-Google providers.
   - A Navbar component with signin/signout UI.
   - Protected pages and an API route as described.
   - Proper TypeScript types (if using TypeScript) and error/loading states.
