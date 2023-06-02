# ChatOverlay
> A Twitch chat overlay for OBS that requires no log-in or additional service like StreamLabs,...

## How To Setup:
- Save the **Chatbox.html** file in a folder of your liking
- Open the file in a text editior
- Search for the line `let channelName = "CHANNEL";` and replace `CHANNEL` with your channel-name as it appears in the link to your channel
- Open OBS, add a new browser source, check the option **Local file** and select the **Chatbox.html** file
- Specify the width and height to your liking

## Some Impressions:
- Current badges: Broadcaster, Mod, Staff, VIP, Partner, Founder, Subscriber\
 ![Badges](/Resources/CurrentBadges.PNG?raw=true "Badges")
 
- In action\
 ![Screenshot](/Resources/Screenshot.PNG?raw=true "Screenshot")

## Planned To-Do List:
- Integrate [Pronouns Extension](https://pronouns.alejo.io/)
- Use custom channel-badges for subs
- Subscription messages / Gift messages

## Version History:
### Version 0.2:
- Added some colorizable badges (broadcaster, staff, mod, vip, verified, sub, founder)

### Version 0.1:
- Username displayed inside a rounded box of their user-color (random if user never picked one)
- Emotes are displayed
- Badges can not be displayed yet, but subscribers are indicated with a heart in front of their name
- Entire message is inside transparent purple-gray box to show above bright backgrounds (shadow looked awful)
- Messages fade-out and get removed from the file after 20 seconds
