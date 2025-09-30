Short Explanation of Each JOIN (Lab Context)

INNER JOIN → Used in /reports/users-with-roles to list users that actually have assigned roles.

LEFT JOIN → Used in /reports/users-with-profiles so all users show up, even if they don’t have a profile.

RIGHT JOIN → Used in /reports/roles-right-join to display every role, even if no user is linked to it.

FULL OUTER JOIN → Used in /reports/profiles-full-outer to combine all users and profiles, showing NULLs when one side is missing.

CROSS JOIN → Used in /reports/user-role-combos to generate every possible user × role combination.

SELF JOIN → Used in /reports/referrals to track which users referred others by joining the users table to itself.

______________________________________________________________________________________________________________
/api Endpoints and Purpose

/users-with-profiles → Shows all users, with profile details if available.

/roles-right-join → Lists all roles and connects them with user_id and email (even roles not assigned).

/profiles-full-outer → Displays all users and all profiles, matched or unmatched.

/user-role-combos → Shows each user paired with every role (student, instructor, admin).

/referrals → Displays who referred whom based on the referral table.

/latest-login → Shows the most recent login activity (timestamp + IP) for each user.
