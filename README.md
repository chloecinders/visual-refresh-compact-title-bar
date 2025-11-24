# Visual Refresh Compact Title Bar

The new Discord theme (also called, and from now on referred to as Visual Refresh) changed the window title bar to be more fat, now also including your inbox, help, and the update button.
This theme aims to move the buttons from the title bar down into the channel header:

Before:
![image](https://github.com/user-attachments/assets/4fd945aa-b31f-4f56-9e67-099efc8b8630)

After:
![image](https://github.com/user-attachments/assets/1a0a3718-dc30-411f-9404-579f5ed65509)

Install:
Use [Vencord](https://github.com/Vendicated/Vencord) or an equivalent client mod that allows you to install themes.

Paste the following link into your online theme links:
```
https://chloecinders.github.io/visual-refresh-compact-title-bar/desktop.css
```

**If you are on a browser, Vesktop, or a client which does not come with window controls paste this instead:**
```
https://chloecinders.github.io/visual-refresh-compact-title-bar/browser.css
```
If you are on browser/Vesktop and do not care about the the inbox button, just wanting a performant way to remove the title bar completely you can use this instead:
```
https://chloecinders.github.io/visual-refresh-compact-title-bar/hidden.css
```

Alternatively if your client does not support online themes you can download one of the theme files found in this repository and put them into your theme folder.

## Config
Put this into your QuickCSS (Or any non-Vencord equivalent) to configure some behavior of this theme:
```css
:root {
    /* controls the vertical position of the window buttons */
    --vr-header-snippet-top: 0px !important;
    /* controls the space above the server list */
    --vr-header-snippet-server-padding: 16px !important;
    /* controls the space the window buttons get on the channel header, experiment around with this if you get gaps or the buttons overlap! */
    --vr-header-snippet-space: 230px !important;
    /* controls the space to the right of the window buttons, good if you are using themes like midnight which add padding to the bar */
    --vr-header-snippet-button-padding: 0 !important;
    /* !DESKTOP SNIPPET ONLY! If set to none instead of flex, hides the window control buttons */
    --vr-header-snippet-winbuttons: flex !important;
}
```
### --vr-header-snippet-space cheat sheet
Try these if you dont want to find out the spacing yourself!

- Desktop Default: 180px
- Desktop Spacious UI Scaling: 200px
- Browser: 85px

