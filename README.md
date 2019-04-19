<img align="left" width="100" height="100" src="https://raw.githubusercontent.com/Jinzulen/Mangadex-RPC/master/ext/icons/mangadex-128.png">

# Mangadex-RPC

[![Build Status](https://scrutinizer-ci.com/g/Jinzulen/Mangadex-RPC/badges/build.png?b=master)](https://scrutinizer-ci.com/g/Jinzulen/Mangadex-RPC/build-status/master) [![Maintainability](https://api.codeclimate.com/v1/badges/990f8b50b19662b84f1a/maintainability)](https://codeclimate.com/github/Jinzulen/Mangadex-RPC/maintainability) [![CodeFactor](https://www.codefactor.io/repository/github/jinzulen/mangadex-rpc/badge/master)](https://www.codefactor.io/repository/github/jinzulen/mangadex-rpc/overview/master) 

Share your reading habits and preferences on Mangadex seemlessly with your friends on Discord thanks to this Discord RPC addon.

### Download & Setup
- **DPS JAR:** [Download from GitHub](https://github.com/Jinzulen/Mangadex-RPC/blob/master/ext/tools/DPS.jar) / [Download on MEGA](https://mega.nz/#!wF43zIQT!KHUNhIuxZnXjvwBjklCqXyNSiNvhyA9hDzm2sz4pyug)
- **Tampermonkey:** [Install Tampermonkey from Chrome Webstore](https://chrome.google.com/webstore/detail/tampermonkey/dhdgffkkebhmkfjojejmpbldmpobfkfo) / [Install Tampermonkey from Firefox Add-ons store.](https://addons.mozilla.org/en-US/firefox/addon/tampermonkey/)
- **Mangadex-RPC:** [Downlaod from GitHub](https://github.com/Jinzulen/Mangadex-RPC/blob/master/src/Mangadex-RPC.js) / [One-click Install via Greasyfork](https://greasyfork.org/en/scripts/381077-mangadex-rpc)

**- How to use:**
1. **Launch DPS**
    - Linux/macOS/Windows: Run the following command on CMD/CLI `java -jar dps-fat-1.0.jar` or right click the file and choose to open it with the Java runtime environment.
    - Once successfully launched, it should return the following message: `Websocket started on port: 6680`
    ![Screenshot of DPS successfully launched on personal Linux machine.](https://i.imgur.com/r76ymXZ.png)
2. **Add the userscript to your prefered injector**
    - Following userscript installation, make sure it is enabled.
3. **Enable game activity on Discord**
    - Go to Discord settings.
    - On the left-hand menu, find Game Activity.
    - Enable "Display currently running game as a status message".
    ![Screenshot of Game Activity enabled on Discord.](https://i.imgur.com/JL2gJ5V.png)
4. **Navigate to [Mangadex](https://mangadex.org/) and open a chapter, any chapter.**
    - Once you open a chapter, a browser notification should appear (after prompting you to allow notifications) to notify you that a DPS connection has been established for that manga.
    - At the same time, if you take a look at the DPS console, you should see it greeting you with a welcome message, such as: `Welcome username#discriminator`

    ![Screenshot of the DPS console greeting me after a successfully websocket connection has been established.](https://i.imgur.com/1FG6dPx.png)

**Note #1:** Your status on Discord must not be set to invisible/offline, otherwise the Rich Presence won't appear.

**Note #2:** If the Rich Presence doesn't appear even though your status isn't set to invisible/offline, then reload Discord.

### Screenshots
![What it looks like on the user profile.](https://greasyfork.org/system/screenshots/screenshots/000/014/769/original/Screenshot_2019-03-28_17-39-43.png?1553794056 "What it looks like on the user profile.") ![What it looks like on the user popup.](https://greasyfork.org/system/screenshots/screenshots/000/014/768/original/Screenshot_2019-03-28_18-01-48.png?1553794056 "What it looks like on the user popup.")

### FAQ
> Firefox is giving me a "Security Error: The operation is insecure." error?
- Firefox does not allow, by default, going from a secure endpoint (https://) to a non-secure one (ws://). This can be disabled by going to `about:config` and changing `network.websocket.allowInsecureFromHTTPS` to `true`.

> I tried to run the DPS JAR but it's giving me some error about tray icons?
- This usually happens if you're using GNOME without the indicators extension installed and enabled.

> I don't really like Tampermonkey, can't I use GM or VM?
- You can use whichever injector you're most comfortable with, I just tend to prefer working with TM.

> Why not include the manga's cover photo in the RPC?
- Unfortunately, that can't be done. RPC assets have to be set in the application's dashboard and are limited to 150 items. Should Discord support an alternative method in the future, I will update the script accordingly.

> Why do I have to download and run some JAR file to get this thing to work? It's so inconvenient!
- Unfortunately, this is the only way to offer an RPC plugin right now. Believe me, I hate adding inconvenient steps to my work just as much as you hate going through them. I can't make any promises but I am studying a few alternative methods for RPC/DPS integration.

### License
[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2FJinzulen%2FMangadex-RPC.svg?type=large)](https://app.fossa.com/projects/git%2Bgithub.com%2FJinzulen%2FMangadex-RPC?ref=badge_large)
