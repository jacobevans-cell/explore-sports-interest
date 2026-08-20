# Explore Academy Season 2 Sports Interest

Files
- index.html — student sports-interest form
- admin.html — live dashboard for viewing responses
- firestore.rules — Firestore rules to paste into Firebase

Firebase setup
1. Firestore Database must be enabled.
2. Authentication > Sign-in method > Anonymous must be enabled.
3. In Firestore > Rules, replace the rules with the contents of firestore.rules and Publish.

GitHub setup
1. Upload index.html and admin.html to the root of:
   jacobevans-cell/explore-sports-interest
2. Go to GitHub repository Settings > Pages.
3. Under Build and deployment, choose:
   Source: Deploy from a branch
   Branch: main
   Folder: / (root)
4. Save.

Pages
Student form:
https://jacobevans-cell.github.io/explore-sports-interest/

Dashboard:
https://jacobevans-cell.github.io/explore-sports-interest/admin.html

Firestore collection
Responses are stored in:
season2SportsInterest

Important
The included Firestore rules allow public read access to this one collection because that is the access model requested for this project. Anyone capable of querying the Firebase project can technically read the collection. Update the rules later if you decide to restrict dashboard access.


Gender eligibility
- Boys only see boys-designated and coed sports.
- Girls only see girls-designated and coed sports.
- 7v7 Passing League is currently configured as coed.
- Esports Mario Kart and Smash Bros are configured as coed.
- Grade 6 can see both Elementary and Junior High categories when applicable.
