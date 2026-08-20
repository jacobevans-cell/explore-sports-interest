EXPLORE ACADEMY ATHLETICS PORTAL — FOUNDATION V1

FILES
index.html                 Master Explore Athletics home
interest.html              Firebase-backed sports interest/enrollment form
admin.html                 Firebase-backed athletics interest/admin dashboard
planner.html               IYAC/CAA budget and team-planning tool
teams/jv-volleyball.html   Existing JV volleyball portal preserved intact
firestore.rules            Current Firestore rules used by interest/admin system

CORE PROGRAM LOGIC
- IYAC first for middle-school opportunities whenever the sport is offered.
- CAA supplements elementary sports IYAC does not appropriately serve.
- 4th grade defaults to CAA elementary.
- 5th grade stays elementary whenever possible even when technically IYAC eligible.
- 6th grade is the bridge grade and is manually placed based on enrollment, roster viability, safety, and competitive balance.
- 7th–8th default to IYAC where available.

CURRENT FOUR-SEASON MODEL
Season 1 Fall: CAA 4–5 Girls Volleyball; IYAC MS Girls Volleyball; IYAC MS Coed Flag
Season 2 Late Fall: CAA 4–6 Boys Volleyball; CAA 4–5 Girls Flag
Season 3 Winter: IYAC MS Boys Basketball; IYAC MS Girls Basketball; CAA 4–5 Boys Flag
Season 4 Spring: IYAC MS Coed Soccer; CAA 4–5 Boys Basketball; CAA 4–5 Coed Soccer if viable

DATE CONFIDENCE
- IYAC Season 1 Sept 21–Nov 19, 2026: confirmed from commissioner information supplied by user.
- CAA sport windows are represented by their published seasonal ranges.
- IYAC basketball/soccer dates are working reconstructed windows until commissioner dates are available.

NEXT ARCHITECTURE PHASE
1. Convert team definitions and league dates into Firestore collections.
2. Create generic team-page template so every sport can have schedule/roster/results like the volleyball hub.
3. Add master athlete records and conflict detection across teams.
4. Add enrollment/consent/payment/status workflow.
5. Add coach assignments, facilities/practice slots, game scheduling, transportation and calendar export.
6. Add automatic viability and CAA cost warnings before team registration deadlines.

BRANDING
The uploaded Sports Calendar project did not contain an official Explore Academy logo image file. The V1 master portal therefore preserves the existing navy/blue/red visual language and uses an eagle mark placeholder. Replace the mark with the official logo when the image asset is available.
