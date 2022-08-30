---
title: "First Run"
date: 2022-08-26T15:45:55+03:00
draft: false
weight: 22
---
Before using simpl:api, there are a few steps to follow to make everything ready.

1. clone the repo
2. In `.env` file, set  `BASE_URL`, `MONGODB_CONNECTION_STRING` and `DB_NAME`
3. In `.env` file, set a UID to `SECRET_KEY`and `NEXTAUTH_SECRET`
4. In `next.config.js` file, set `baseUrl` and `secretKey` according to `.env` file.
5. Start simpl:api with `npm run dev` command.
6. In your browser, enter `/api/v1/install/first-run`. This will create required db collections and admin account and will return credentials to your browser as response. Delete this folder after all steps are done.
7. In your browser, enter `api/v1/key/generate`. This page is protected with authentication, so you have to use your admin credentials which were created previous step.
8. Copy generated API key from your browser and paste it to api key variable in both `.env ` and `next.config.js` file
9. Restart the server (Ctrl+C then run the command from step 5)
10. Congratulations ! simpl:api is ready to use! 😀

{{< hint type=warning icon=gdoc_fire title="Change Admin credentials" >}}
After completing all steps, please change admin credentials through the dashboard.
{{< /hint >}}

{{< hint type=warning icon=gdoc_fire title="Delete Installation Folder" >}}
After completing all steps, please delete installation folder from /pages/api/v1/install.
{{< /hint >}}

{{< hint type=important icon=gdoc_error_outline title="Don't share secret key" >}}
Secret key protects some senstive api routes (such as creating, editing, deleting routes), don't share secret key that doesn't have admin rights.
{{< /hint >}}
