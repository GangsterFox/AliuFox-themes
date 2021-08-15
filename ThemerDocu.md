# Themer Docu for the xposed/plugin
This is a docu for dark mode theming, be welcome to add things to the docu! I would be really happy
* [License](https://github.com/GangsterFox/AliuFox-themes/blob/main/LICENSE)

<h1 align="center">Misk Strings for Plugin</h1>

* Strings used for the plugin to tell the user what the name of the theme is, author, version, license, etc but also things like custom font and custom background

```json
{
    "name": "theme name",
    "author": "author name",
    "version": "1.0.0, will be used by updater in the future",
    "updater": "updater url (must be raw url) not actually implemented yet lol",
    "license": "license, not implemented into the ui",
    "background": "url of background, default transparency is set to 150 in plugin",
    "background_transparency": 0 (fully transparent, number goes from 0 to 255),
    "font": "link to the font, can be any cdn link. You can use a .tff or a .otf"
}
```

<h1 align="center">Brand/Accent Colors</h1>

* Accent colors

| String          | Purpose                 |
| ---------------- |:-----------------------:|
| brand up to 900 | old brand colors, are not used anymore so they are useless |
| brand_new up to 900 | new brand colors |
| brand_new | accent color |
| brand_new 230 to 630 | accent colors for buttons, bot tags, on/off sliders blah blah |
| brand_new_560 | change the reaction clicked border |
| link | literally just link colors and mention color |

<h1 align="center">Primary Colors</h1>

* Primary colors, used for the big things chat bg, server list, member list, etc

| String          | Purpose                 |
| ---------------- |:-----------------------:|
| primary_600 | server folders and something else I have no idea xdddd |
| primary_700 | spoilers,emebeds,top bar, DMs Button, bg for pings and server streaming icons (in plugin only changes the DMs button and also top bar) |
| primary_dark_600 | main chat bg and also somehow changes the member list bg |
| primary_630 | channel header and a lot of other stuff(use primary_dark_630 since it somehow changes all of this stuff too in plugin) |
| primary_dark_400 | changes the text "Message #..." color and also timestamp color also changes the status text in member list |
| primary_dark_660 | color for the chat bar where you write your messages, also changes the icon bg for gifts and attachment |  
| primary_dark_800 | color for the bottom bar in the channel list, where the icons for friends, search, mentions, etc is |
| primary_dark_700 | server list |
| primary_800 | file select tab thing where you can choose from images, files, photots or go back to keyboard |

<h1 align="center">uikit Strings</h1>

* uikit strings. They are in the Color Values screen if you dont know

| String          | Purpose                 |
| ---------------- |:-----------------------:|
| uikit_btn_bg_color_selector_brand | changes buttons in general so send button for example |
| uikit_btn_bg_color_selector_green | change color for the online icon |
| uikit_btn_bg_color_selector_red | changes the ping color |

<h1 align="center">Drawable Strings</h1>

* Drawable strings, used in a lot of places

| String          | Purpose                 |
| ---------------- |:-----------------------:|
| drawable_button_grey | unread messages button |
| item_background_material | mostly used for the top bar(where the name of the plguin, version and author name is written) |
| design_bottom_navigation_item_background | is used mostly for the bottom part for plugin page(where description is, uninstall and settings) also themes search box in plugins page |
| ic_channel_text | by the name it changes the channel text in the channel list, since it doesnt get themed it will only theme the # in the channel list and top bar when looking in chat |
| drawable_button_red | the red NEW↑ in the guild list when you get a ping in a guild |
| drawable_button_red_neutral | I actually have no idea what it does, if you find anything please tell me, thanks. |
| drawable_voice_indicator_speaking | the color for the ring when someone talks in a vc |
| drawable_voice_user_background_speaking | speaking background, I dont know how to better explain it |
| drawable_voice_sensitivity_progress | the progress bar for when you test out your mic sens |
| ic_ban_red_24dp | the ban icon color, kind of pointless tbh and no I dont know what the kick icon color string like at all |

<h1 align="center">Links for experienced Users</h1>

* This link by ven might help you if you know what you are doing

https://gist.github.com/Vendicated/7e8aa7b2512b8e38e041692cbf34acfa
