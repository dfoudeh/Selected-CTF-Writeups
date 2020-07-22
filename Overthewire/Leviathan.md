# Leviathan

## Leviathan0

In the home directory we find a hidden folder .backup that has a bookmarks.html File. Greping the file for leviathan we find the password for leviathan1.

## Leviathan1

In the home directory we find an executable named check. When we run it, it prompts us for a password. I ran `ltrace ./check` and entered test for password. `strcmp("tes", "sex")` We can see that  there is a call to strcmp checking the first 3 chars of our password agaisnt sex. Running again and using sex as our password, we are prompted with a different shell. Running `whoami` tells us that we are logged in as leviathan2. We are told earlier that user passwords live in `/etc/leviathan_pass`; looking in leviathan2 gets us the password.