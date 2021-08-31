# Themer Docu for the xposed/plugin
This is a docu for dark mode theming, be welcome to add things to the docu! I would be really happy
* [License](https://github.com/GangsterFox/AliuFox-themes/blob/main/LICENSE)

<h1 align="center">Misc Strings for Plugin</h1>

* Strings used for the plugin to tell the user what the name of the theme is, author, version, License, etc but also things like custom font and custom background

```json
{
    "name": "theme name",
    "author": "author name",
    "version": "1.0.0, version for theme, used for updater string",
    "updater": "updater url (must be a raw.githubusercontent.com url). Needs version bump if you update your theme",
    "license": "license, not implemented into the ui",
    "background": "url of background",
    "background_transparency": 0,
    "font": ""
}
```
* Info on background transparency: 0 is fully transparent while 255 is fully opaque. The default transparency setting used in the plugin is 150
* Info on font: please use a cdn link. I recommend you to use cdn.discord.com or raw.githubusercontent.com. Use a .ttf file or a .otf
* Info on background: Image formats like png, jpg, jpeg should work. Animated png's or any animated formats **do not work as of now** 
* Info on updater: it will only work with github as far as I know, so if you want your themes to get automatically updated, please set up a repo with your themes

<h1 align="center">Brand/Accent Colors</h1>

* Accent colors

| String          | Purpose                 |
| ---------------- |:-----------------------:|
| brand up to 900 | old brand colors, are not used anymore, so they are useless |
| brand_new up to 900 | new brand colors |
| brand_new | accent color |
| brand_new_360 | changes the cursor when typing color, bare in mind this WILL change the nitro text color in the settings, the turned on switch(best seen in plugins page) and probably more |
| brand_new 230 to 630 | accent colors for buttons, bot tags, on/off sliders blah blah |
| brand_new_560 | change the reaction clicked border |
| link | literally just link color |

<h1 align="center">Primary Colors</h1>

* Primary colors, used for the big things chat bg, server list, member list, etc

| String          | Purpose                 |
| ---------------- |:-----------------------:|
| primary_600 | server folders and something else I have no idea xdddd |
| primary_700 | spoilers,embeds,top bar, DMs Button, bg for pings and server streaming icons (in plugin only changes the DMs button and also top bar) |
| primary_dark_100 | changes chat scroll bar |
| primary_dark_600 | main chat bg and also somehow changes the member list bg |
| primary_630 | channel header |
| primary_dark_630 | channel list |
| primary_dark_200 | changes text color for main text |
| primary_dark_400 | "Message #..." color, timestamps, user statuses, UserDetails texts, TextInput placeholders (chat, searchbars), Guild/Category name in search tab, new day divider lines in chat |
| primary_dark_660 | color for the chat bar where you write your messages, also changes the icon bg for gifts and attachment |  
| primary_dark_800 | color for the bottom bar in the channel list, where the icons for friends, search, mentions, etc is |
| primary_dark_700 | server list |
| primary_800 | file select tab thing where you can choose from images, files, photos or go back to keyboard |

<h1 align="center">uikit Strings</h1>

* uikit strings. They are in the Color Values screen if you dont know

| String          | Purpose                 |
| ---------------- |:-----------------------:|
| uikit_btn_bg_color_selector_brand | changes the settings button in settings like in the plugin list or dev options the 4 at the bottom |
| uikit_btn_bg_color_selector_green | change color for the online icon |
| uikit_btn_bg_color_selector_red | changes the ping color and in plugin list the uninstall button, also changes color for the "NEW MESSAGES" in chat |
| uikit_btn_color_selector_background_accent_dark | changes muted channel color in channel sidebar, the thread spine, the blobs when member list is loading and also the emote picker selected for emoji/GIFs/Stickers(also changes the text color of the emoji/GIFs/Stickers) |

<h1 align="center">Drawable Strings</h1>

* Drawable strings, used in a lot of places

| String          | Purpose                 |
| ---------------- |:-----------------------:|
| drawable_button_grey | unread messages button |
| drawable_overlay_channels_selected_dark | Selected channel color in channel list for dark mode |
| item_background_material | mostly used for the top bar(where the name of the plugin, version and author name is written) |
| design_bottom_navigation_item_background | is used mostly for the bottom part of the plugin page(where description is, uninstall and settings) also themes search box in plugins page |
| ic_channel_text | by the name it changes the channel text in the channel list, since it doesn't get themed it will only theme the # in the channel list and top bar when looking in chat |
| drawable_button_red | the red NEW↑ in the guild list when you get a ping in a guild |
| drawable_button_red_neutral | I actually have no idea what it does, if you find anything please tell me, thanks. |
| drawable_voice_indicator_speaking | the color for the ring when someone talks in a vc |
| drawable_voice_user_background_speaking | speaking background, I don't know how to better explain it |
| drawable_voice_sensitivity_progress | the progress bar for when you test out your mic sens |
| ic_ban_red_24dp | the ban icon color, kind of pointless tbh and no I don't know what the kick icon color string like at all |

<h1 align="center">Links for experienced Users</h1>

* This link by ven might help you if you know what you are doing

https://gist.github.com/Vendicated/7e8aa7b2512b8e38e041692cbf34acfa

<h1 align="center">Light mode theming</h1>

* The way to theme in light mode is to find as many strings which have the word "light". This means for example if you find primary_light, that means you found a light mode string.
* This might be quite weird to do since this is some territory no one has really tried yet. Bare in mind this might not work on plugin but dont take my word.
* When you try to theme in light mode, at least with primary colors, try to use the same strings as written in the docu but try to add the _light string. 
* **Always** search before you do anything to find strings.
* This means that if you will try theming in light mode, just try to add _light to the string
* And as always, Good luck
*this will get updated when I will found out more.* 
