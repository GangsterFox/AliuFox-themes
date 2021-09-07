# Themer Docu for the xposed/plugin
This is a docu for dark mode theming, be welcome to add things to the docu! I would be really happy
* [License](https://github.com/GangsterFox/AliuFox-themes/blob/main/LICENSE)

<h1 align="center">Misc Strings for Plugin</h1>

**DO NOT CHANGE THE JSON DIRECTLY UNLESS YOU KNOW WHAT YOU ARE DOING, I AM NOT GOING TO GIVE YOU SUPPORT IF YOU DO CHANGE DIRECTLY.
INSTEAD USE THEMERS EDITOR TO ADD THINGS TO THE STRINGS**

> Strings used for the plugin to tell the user what the name of the theme is, author, version, License, etc but also things like custom font and custom background


* The manifest strings

Used to show name of the theme, author, etc. They are in the "manifest" section in the .json
```json
{
  "name": "the theme name",
  "author": "authors name",
  "license": "license, ask if you want to add one but dont know how to or what license to choose in #theme-development",
  "version": "this is the verion number, DO NOT USE TEXT AS A VERSION BECAUSE THIS **WILL** BREAK THE UPDATER AND WONT UPDATE YOUR THEME AT ALL",
  "updater": "this is where you put your raw.githubusercontent.com link, if you ever want to update your theme just bump the version number up"
}
```
When done correctly it should look like this in the json
![image](https://user-images.githubusercontent.com/84905506/132266565-ff27a087-4e36-48ca-baca-2a1d823939fd.png)

* Background strings

These are the strings for adding a background and also giving it transparency(alpha). They are in the "background" section in the .json
```json
{
  "url": "url for the bg image, recommended and trusted to use cdn.discordapp.com links",
  "alpha": "background transparency, goes from 0 to 255, 0 being fully transparent while 255 being fully opaque"
}
```
When done correctly it should look like this in the json
![image](https://user-images.githubusercontent.com/84905506/132266685-eaa4cca8-9d49-449a-bf8b-c17acc9d3270.png)
* Font string

The string for the font URL. The string is located in the "fonts" section in the .json
```json
{
  "*": "url of the font, recommended and trusted to use cdn.discordapp.com links"
}
```
When done correctly it should look like this in the json
![image](https://user-images.githubusercontent.com/84905506/132266358-3d8e34da-622d-49d9-b74a-d7dd1d413ee6.png)
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

<h1 align="center">Primary dark Colors</h1>

* Primary dark colors, used for the big things chat bg, server list, member list, etc for dark mode

| String          | Purpose                 |
| ---------------- |:-----------------------:|
| primary_dark_100 | changes chat scroll bar |
| primary_dark_300 | in the plugin: changes icons color for attachments and emotes icon, DMs button, discord navagation button colors, top bar icons, member list icons (only changes the search icon and settings icon in member list), changes the text under the icons(search, pins, etc) for member list, changes the text for the names of roles in member list, changes server name color in the emotes list and icons for default emotes. |
| primary_dark_360 | only in plugin: changes the read channel names and the icon next to them, also changes peoples names in the DM list [example](https://cdn.discordapp.com/attachments/590317150959566849/884594678832455770/Screenshot_20210907-022053.jpg) |
| primary_dark_600 | main chat bg and also somehow changes the member list bg |
| primary_dark_630 | channel list |
| primary_dark_200 | changes text color for main text |
| primary_dark_400 | "Message #..." color, timestamps, user statuses, UserDetails texts, TextInput placeholders (chat, searchbars), Guild/Category name in search tab, new day divider lines in chat |
| primary_dark_660 | color for the chat bar where you write your messages, also changes the icon bg for gifts and attachment |  
| primary_dark_800 | color for the bottom bar in the channel list, where the icons for friends, search, mentions, etc is |
| primary_dark_700 | server list |

<h1 alight="center">Primary strings</h1>

* Primary strings used for both dark and light mode, used for smaller things

| String          | Purpose                 |
| ---------------- |:-----------------------:|
| primary_600 | server folders and something else I have no idea xdddd |
| primary_700 | spoilers,embeds,top bar, DMs Button, bg for pings and server streaming icons (in plugin only changes the DMs button and also top bar) |


<h1 align="center">uikit Strings</h1>

* uikit strings. They are in the Color Values screen if you dont know

| String          | Purpose                 |
| ---------------- |:-----------------------:|
| uikit_btn_bg_color_selector_brand | changes the settings button in settings like in the plugin list or dev options the 4 at the bottom |
| uikit_btn_bg_color_selector_green | change color for the online icon |
| uikit_btn_bg_color_selector_red | changes the ping color and in plugin list the uninstall button, also changes color for the "NEW MESSAGES" in chat |

<h1 align="center">Drawable Strings</h1>

* Drawable strings, used in a lot of places

| String          | Purpose                 |
| ---------------- |:-----------------------:|
| drawable_button_grey | unread messages button |
| drawable_overlay_channels_selected_dark | Selected channel color in channel list for dark mode |
| drawable_overlay_channels_pressed_dark | Pressed channel color in channel list for dark mode | 
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
