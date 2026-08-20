Explore Academy Season 2 Sports Interest — Corrected Offerings

STUDENT FORM
Students can choose a maximum of TWO sports.
They must identify a FIRST choice.
The second selection is treated as a backup choice.
The form clearly explains that all teams depend on participation numbers.

AVAILABLE PROGRAMS

IYAC
- Coed Flag Football — Grades 5–8
- Boys and girls play together.

CAA
- Boys Volleyball — Grades 4–8 interest pool
  - CAA has overlapping 4–6 and 6–8 divisions.
  - 6th graders select Boys Volleyball only once.
  - Final team/division placement is determined after participation numbers are reviewed.
- Girls Flag Football — Grades 4–5

INTERNAL
- Esports: Mario Kart — Grades 4–8, coed
- Esports: Smash Bros. — Grades 4–8, coed

The form filters choices automatically by grade and gender.

FILES
- index.html — corrected student interest form
- admin.html — results dashboard
- firestore.rules — existing Firestore rules

FIREBASE
No database reset is required.
New responses will use the corrected sport names and include firstChoice and secondChoice fields.

GITHUB
Replace index.html and admin.html in the repository root.


CLEAR ALL RESPONSES BUTTON
- admin.html now includes a Clear All Responses button.
- It requires typing: DELETE ALL RESPONSES
- It then requires a second browser confirmation.
- The included firestore.rules allows deletes from the season2SportsInterest collection.
- IMPORTANT: Because the dashboard is not login-protected, delete access is also not identity-restricted. The typed confirmation prevents accidents but is not true access control.
- Publish the updated firestore.rules before using the clear button.


ROSTER SETUP
- The supplied Grades 4–5 and Middle School rosters are preloaded into index.html and admin.html.
- Admin Dashboard > Roster Setup lets you multi-select students.
- Choose a grade, gender, or both, then click Apply to Selected.
- Use the roster-group filter and Select Visible for batch work.
- Student form now uses a student-name dropdown.
- If roster metadata has been saved, grade and gender auto-fill when a student chooses their name.
- If metadata has not been saved yet, grade/gender remain manually selectable.
- Roster metadata is stored in Firestore collection: sportsRoster.
- Publish the included updated firestore.rules before using Roster Setup.


V6 BULK RESPONSE ENTRY
- Roster Setup now includes grade, gender, and name filters.
- Example workflow:
  1. Filter Grade 4.
  2. Filter Girls.
  3. Click Select Filtered.
  4. Choose CAA Girls Flag Football.
  5. Click Create Responses.
- One Firestore response is created for every selected student.
- Eligibility is checked before the records are created.
- You can also assign one first choice plus one second choice to the whole selected batch.
