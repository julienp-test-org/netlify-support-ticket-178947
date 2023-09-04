# netlify-support-ticket-178947

Each of `site1`, `site2`, and `site3` are the demo Next.js sites. `site2` is configured to exit with a status of 1 after sleeping for 60 seconds.

Create a new PR modifying the readme in `site2`, and you should see the check for `site1` show as cancelled, and `deploy/netlify` should pass, allowing the merge. 

Then, as soon as the check for site 2 fails, the `deploy/netlify` check will fail, preventing merge.