# kubernetes-matrix-dimension-install

Proper `accessToken` must be provided, in order to connect dimension to synapse.
Explanation copy+pasted from here: [https://t2bot.io/docs/access_tokens/](https://t2bot.io/docs/access_tokens/)

0. Create account that would be used as a bot.
1. In a private/incognito browser window, open Riot.
2. Log in to the account you want to get the access token for, such as the bot's account.
3. Click on the bot's name in the top left corner then "Settings".
4. (Optional) Set your bot's display name and avatar.
5. Click the "Help & About" tab (left side of the dialog).
6. Scroll to the bottom and click the <click to reveal> part of Access Token: <click to reveal>.
7. Copy your access token to a safe place, like the bot's configuration file.
8. Do not log out. Instead, just close the window. If you used a private browsing session, you should be able to still use Riot for your own account. Logging out deletes the access token from the server, making the bot unable to use it.
9. Insert obtained `accessToken` into config:
```
      # The access token Dimension should use for miscellaneous access to the homeserver, and
      # for tracking custom sticker pack updates. This should be a user configured on the homeserver
      # and be dedicated to Dimension (create a user named "dimension" on your homeserver). For
      # information on how to acquire an access token, visit https://t2bot.io/docs/access_tokens
      accessToken: "MDAyNWxvY2F0aW9uIHN5bmFwc2Uuc3Vuc2luZ2VydXMuY29tCjAwMTNpZGVudGlmaWVyIGtleQowMDEwY2lkIGdlbiA9IDEKMDAzNWNpZCB1c2VyX2lkID0gQGRpbWVuc2lvbjpzeW5hcHNlLnN1bnNpbmdlcnVzLmNvbQowMDE2Y2lkIHR5cGUgPSBhY2Nlc3MKMDAyMWNpZCBub25jZSA9IENQcGZFa21wWmcuVX5QOlkKMDAyZnNpZ25hdHVyZSB7aVgNJ-NnguroqjOF7skq2lPiA0Kf9XeV2n9_EaFTJwo"
```



How to install matrix-dimension on kubernetes

Installation instructions
[https://github.com/turt2live/matrix-dimension/blob/master/docs/installing.md](https://github.com/turt2live/matrix-dimension/blob/master/docs/installing.md)

Dockerile
[https://hub.docker.com/r/turt2live/matrix-dimension/dockerfile](https://hub.docker.com/r/turt2live/matrix-dimension/dockerfile)


Take a look into [https://t2bot.io/docs/access_tokens/](https://t2bot.io/docs/access_tokens/) for explanation on how to get access code for Dimension to access Synapse
