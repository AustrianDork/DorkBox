# ChatOverlay
> A Twitch chat overlay for OBS that requires no additional log-in service like StreamLabs,...

## How To Setup:
- Save the **Chatbox.html** file in a folder of your liking ([Latest Release Here](https://github.com/AustrianDork/DorkBox/releases/latest))
- Open the file in your browser of choice
- Click on the address bar to edit the "url" (should read something like `file:///.../Chatbox.html`)
  - **Required:** Add `?channel=YourChannelName` and enter your channel name as it appears the link to your stream
  - **Optional:** If you want to display [Pronouns](https://pronouns.alejo.io/) (off by default), add `&pronouns=true`
  - **Optional:** If you want to change the message fade-out delay (default is 30 seconds), add `&delay=NumberInSeconds`
  - **Optional:** If you want to change the scale (default is 1), add `&zoom=ScaleNumber`
- Add a new browser source in OBS and just copy the whole "url" \
 (something like `file:///.../Chatbox.html?channel=twitch&pronouns=true&delay=120&zoom=1.75`) into the URL field
 
## What it looks like:
- Minimalistic, instant-messenger-esque appearence
- Displays animated and static emotes
- Current badges: Broadcaster, Mod, Staff, VIP, Partner, Founder, Subscriber, Artist\
 ![Badges](/Resources/CurrentBadges.PNG?raw=true "Badges")
- Pronouns are displayed like this:\
 ![Pronouns](/Resources/Pronouns.PNG?raw=true "Pronouns")
- Changing the scale looks like this:\
 ![ZoomIn](/Resources/ZoomIn.PNG?raw=true "ZoomIn")\
 ![ZoomOut](/Resources/ZoomOut.PNG?raw=true "ZoomOut")
- In action:\
 ![Screenshot](/Resources/Screenshot.PNG?raw=true "Screenshot")
 
## Planned To-Do List:
- Use custom channel-badges for subs (difficult; Twitch API wants credentials for that)

## Version History:
### Version 0.3:
- Reworked the setup to allow for easier settings and updating in the future
    - For future updates, just replace the HTML file with the new one and it'll work with the same browser source
- Added option to display user pronouns
- Added option to change the message fade-out delay
- Added option to change the scale
    - Zooming in (values larger than 1) or zooming out (values smaller than 1)
- Added subscription and gift notification
- Added artist badge
### Version 0.2:
- Added some colorizable badges (broadcaster, staff, mod, vip, verified, sub, founder)
### Version 0.1:
- Username displayed inside a rounded box of their user-color (random if user never picked one)
- Emotes are displayed
- Badges can not be displayed yet, but subscribers are indicated with a heart in front of their name
- Entire message is inside transparent purple-gray box to show above bright backgrounds (shadow looked awful)
- Messages fade-out and get removed from the file after 20 seconds
