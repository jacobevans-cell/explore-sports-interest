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
