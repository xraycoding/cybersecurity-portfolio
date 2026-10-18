\# Non-Root Admin User: Stop Using Root



\## Goal

Do all daily work as a limited identity, so root stays locked away.



\## Part 1: Created the user and group



I created an admin group with the required policy attached to the group, not directly to the user, then created my user and added it to the group.



!\[IAM users list showing one user that belongs to one group](../assets/admin-user-in-group.png)



The IAM users list shows one user and a Groups count of 1, which confirms the user gets its permissions through a group rather than being granted them directly.



\## Part 2: Enabled MFA on the new user



Same approach as root: authenticator app, confirmed with two codes.



\## Part 3: Signed in as the admin user



I signed out of root and logged in as the new user to confirm everything I need works without root.



\## What I learned

\- Permissions through groups are easier to manage than attaching them per user.

\- Full admin is still broad. A later improvement is moving to least-privilege policies.

