# basic-privacy
A quick rundown of basic better privacy apps and operating system changes

## Windows Devices

Windows is a extremely non-private OS, with a large amount of data being shared with Microsoft by default (and more of it with each passing OS update).  This is a non-exhaustive list of at lease easy-ish changes that can be made to help, but the best prevention is to use Linux, or OSX (which is a measure better but not perfect) if Linux is too frightning.

### Application management and updates

Before you start replacing any appliations, you need to have some method to manage your installed applicationas and keep them updated.  

Download and install [UniGetUi](https://github.com/marticliment/UniGetUI/releases/latest).  It is able to see, install, update, and uninstall nearly every application and package on a Windows OS.

Once you have it installed, see below for the recommended settings.  

Once you have the settings set, click on Software Update and update all of the outdated packages it found.

NOTE: Some packages will fail to update.  This is just the nature of some Windows software.  You can clikc on the error at the bottom of the window to see the details.  If the error says "use the applications update method" then you can ignore updates for the package (right click on the application and click 'ignore updates') and it won't try to manage it again and let the application take care of it.

#### UniGetUi Settings

A few setting tweaks you probably want to make when you install UniGetUI.  Glick on the 'Gear' (Settings) Icon on the left bar to access the settins menu

* General Preferences :: Manage Tellemetry Settings
  * Decline this is you are paranoid.  Leave it on to help the devs
* Startup Options :: Enable Scoop Cleanup At Launch :: On
* Insall and Update Preferences 
    * Check for Updates every :: 1 day
    * Optional :: Ask to delete desktop shortcuts (if you don't like application installers leaving shortcuts all over your desktop)
* Administrator Priveleges Prefernces
    * Ask for administrator priveleges once for each batch of operations


### Browser Applications

Use either [Brave](https://brave.com/download/) (for Chromium-based experience seekers) and/or [LibreWolf](https://librewolf.net/installation/windows/) (for a Fire-fox like experience).

Warning: More and more websites are designed explicitly to work with Chromium-like browsers.  So for the best chance at compatablity with the most websites, install just Brave.  If you like Firefox I'd install both LibreWolf and Brave for the occational site that does not work with LibreWolf.  

### Brave install and settings

WARNING: Brave pushing some block-chain technology really hard, especially their own block chain token called BAT.  You can completely ignore this if you are not insterested in any block-chane or token based features. 

* Install using UniGetUi if you have it

Setttings that need to be changed.  Click on the 'Burger' menu and then 'settings'

Getting Started

* Default browser: Click "Make Default" (unless you want Librewolf, then don't)
* On Startup: Continue where you left off
    * OR: for paranoid 'Open the new tab page'
* New Tab page shows: Select "blank page"

Apperance

* Show brave News Button: Off
* Show Leo AI Button: Off (unless you absolutely need an AI assistant)
* Show Brave Rewards button: Off
* Show Brave Wallet Button: Off
* Show VPN button: Off
* Always show full URL: On
* Optional: Use vertical tabs: Off (if you like the classic horizontal tabs)

Content (all optional)
* Show wayback machien prompt on 404 pages: On
* Speedreader: On (optional - may break some sites)

Shields
* Block finterprinting: On
* Block Cookeies: Block thrid-party cookies (will break some sites, you can make site-by-site expections by clikc on the brave shield icon in the address bar when on the broken site)
* Optional paranoid: Forget me when I close this site: On for paranoid
  * WARNING: This means ever time you visit a site with a login, you'll need to log in again
* Allow facebook logins and embeded posts: Off
  * WARNING: Will break some facebook content on non-FB sites
* Allow X (twitter) embeded tweets: Off
  * WARNING: Will break some X content on non-X sites
* Allow LinkedIn embedded posts: Off
  * WARNING: Will break some LinkedIn content on non-LI sites

Privacy and Securtiy

* Delete browsing data : On Exit tab
  * Optional: Browsing history (paranoid only)
    * WARNING: This will log you out of all websites every time you close your browser
  * Leo AI: Checked (unless you use this extensively)
  * Chached images and files
  * Autofill form data
  * Hosted app data
* Security
  * Safe Browsing: Standard Protection
  * Use Secure DNS: On
  * Select DNS Provider: Cloudflare (1.1.1.1)
* Use google services for push messaging: Off
* Auto-redirect AMP pages: On
* Auto-redirect tracking URLs: On
* Prevent sites from fingerprinting me based on my language prefrences: On
* Send a do not track requests with browsing traffic: On (click confirm on the warning box)
* Allow privacy-presering product analitics: On for paranoia
* Automatically send daily usage ping to brave: Off
* Automatically send diagnostic reports: Off

Web 3 (settings are for non-block-chain users)
* Enable NFT discovery: Off
Enable brafe wallet in private windows: off

Leo
* Show leo icon in sidebar: Off
* Show leto in context menu on websites: Off
* Store my conversation history: off

Sync
* If you are going to use Brave on another device (including moble) you'll need to set this up.  Make sure you store your sync passphrase in a password manager!!!

Search Engine
* Normal Window: DuckDuckGo
* Private Window: DuckDuckGo
* Show search suggestions: Off
* Web Discovery Project: Off
* Index other search engines: Off

Extensions
* Allow Google login for extnsion: Off (unless you pay for an extension with your google account)
* Media Router: Off (unless you want to use Andoid's CAST feature to send data to this browser)
* WebTorrent: On
* Widevine: On (needed for watching streaming media)

Autofill and passwords (use Bitwarden or another seperate password manager instead of this feature)
* Payment Methods
  * Turn all setings off
* Addresses and more
  * Turn all settings off

System
* Continue running background apps when brave is closed: Off
* Memory save: On (balanced)
* Energy Save: On (turn on when computer is unplugged)

### Brave Extensions

NOTE: Brave has built in add blocking and URL filtering so you don't need uBlock/uBlockOrigin

Go to the [web store](https://chrome.google.com/webstore/category/extensions) and install

* [BitWarden](https://chromewebstore.google.com/detail/bitwarden-password-manage/nngceckbapebfimnlniiiahkandclblb) (or your password manager of choice)

## iOS Devices

### Maps

In theory Apple Maps is OK due to Apple's privacy commitments, however with the erosion of some of their privacy measures, especially in the EU, it may be a good idea to uninstall Apple Maps and use [Organic Maps](https://apps.apple.com/us/app/organic-maps-offline-map/id1567437057) instead

## Android Devices

### Maps

Use [Organic Maps](https://play.google.com/store/apps/details?id=app.organicmaps&hl=en-US&pli=1) instead of Google maps

* Why: Google Map location history tracking, even though you can set it to auto-prune, is still a tremendous security issue
* Organic Maps is a completely offline map application that never sends your location data to Google's servers
* Your location can still be tracked via your phone's location tracking service and via cell tower tracking, but it at least takes away a major database of your location istory