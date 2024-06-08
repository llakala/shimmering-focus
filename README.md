# Shimmering Focus ⟡
![Download count](https://img.shields.io/badge/downloads-166445-6E4E9B?style=plastic&logo=obsidian&color=%23483699)
![Last commit](https://img.shields.io/github/last-commit/chrisgrieser/shimmering-focus?style=plastic)
![Changelog](https://img.shields.io/badge/changelog-here-6E4E9B?style=plastic&color=%23f6c66f)

A minimalistic and opinionated Obsidian theme for the keyboard-centric user.  
[🏆 Winner Obsidian October 2022 (Category: Theme Update)](https://forum.obsidian.md/t/obsidian-october-2022-winners/49087).

![Promo screenshot](assets/promo-screenshot-big.png)

---

<!-- toc -->

- [Features](#features)
	* [Design philosophy](#design-philosophy)
	* [Select theme features](#select-theme-features)
	* [Commands](#commands)
	* [Create your own color scheme](#create-your-own-color-scheme)
- [Credits](#credits)
	* [Licenses](#licenses)
	* [Thanks](#thanks)
	* [About the developer](#about-the-developer)

<!-- tocstop -->

## Features

### Design philosophy
- __Radical minimalism:__ As opposed to a minimalism of *colors*, this theme
  focuses on a minimalistic *user interface*: Buttons and sidebars not relevant
  for keyboard users are removed. UI elements that require the mouse are still
  accessible on hover. All hidden UI elements can be permanently re-enabled
  with the [Style Settings
  Plugin](https://obsidian.md/plugins?id=obsidian-style-settings).
- __Condensed Display of Information:__ Unnecessary padding and white-space is
  removed, which is beneficial for small screens or higher zoom levels.
- __High Customizability:__ Dozens of customization options available via the
  [Style Settings Plugin](https://obsidian.md/plugins?id=obsidian-style-settings).

![Explaining screenshot](assets/explainer-screenshot.png)

### Select theme features
- Emphasis of __Pandoc Citations__ and __Footnotes__.
- __Alt-text of images__ is used as __caption__.
- Images can be __zoomed in__ by clicking and holding. You can also toggle
  between reduced and original size via command (requires Style Settings
  Plugin).
- __Writing__: Extensive styling for the [Longform
  Plugin](https://obsidian.md/plugins?id=longform), including alternative
  background colors and the use of serif-fonts only inside longform projects.
- __Vim mode__: Explicit styling of Obsidian's Vim Mode and various style
  settings for vim mode, such as relative line numbers.
- __Tables__: Highlighting of active cells, alternating row colors
- Dozens of customization options available via [Style
  Settings Plugin](https://obsidian.md/plugins?id=obsidian-style-settings).
- …and more many more.

> [!NOTE]
> This theme only supports the Obsidian desktop release. PRs with fixes for
> mobile are welcome though.

### Commands
When the [Style Settings
Plugin](https://obsidian.md/plugins?id=obsidian-style-settings) is installed,
Shimmering Focus adds commands for toggling theme features:
- Toggle folding of URLs (Source Mode)
- Toggle between reduced and original image size (reduced size can be set in the
  respective style setting)

### Create your own color scheme
With *Shimmering Focus*, you can create your own color scheme with this CSS
snippet. You are welcome to [share your color
scheme](https://github.com/chrisgrieser/shimmering-focus/discussions/new?category=share-your-custom-color-schemes).

```css
.theme-light.theme-light {
    --bg-hue: 230;
    --bg-sat: 25%;

    /* `--color-accent-hsl` should have the same values as `--color-accent` */
    --color-accent: hsl(184 79% 35%);
    --color-accent-hsl: 184, 79%, 35%;
    --interactive-accent: hsl(184 79% 30%);

    --alt-heading-color: hsl(232 34% 50%);
    --secondary-accent: hsl(28 54% 51%);
    --hover-accent: hsl(328 100% 54%);
    --link-unresolved-color: hsl(101 42% 51%);
}

.theme-dark.theme-dark {
    --bg-hue: 230;
    --bg-sat: 15%;

    /* Note that `--color-accent-hsl` should have the same values as `--color-accent` */
    --color-accent: hsl(184 79% 45%);
    --color-accent-hsl: 184, 79%, 35%;
    --interactive-accent: hsl(184 79% 30%);

    --alt-heading-color: hsl(232 50% 70%);
    --secondary-accent: hsl(28 63% 61%);
    --hover-accent: hsl(328 100% 64%);
	--link-unresolved-color: hsl(101 42% 51%);
}

/* Hide the background color settings since they are overwritten by the custom colors above */ 
.style-settings-container .setting-item:is([data-id="bg-hue-light"],[data-id="bg-hue-dark"]) {
	display: none;
}
```

## Credits

### Licenses
- This theme is licensed under the [MIT
  License](https://github.com/chrisgrieser/shimmering-focus/blob/main/LICENSE).
- The two embedded fonts *iA Writer Quattro* and *Recursive* are licensed under
  the [SIL Open Font License](https://www.wikiwand.com/en/SIL_Open_Font_License).
- The embedded *Material Icon* font is licensed under the [Apache License](https://developers.google.com/fonts/docs/material_icons#licensing).

<!-- vale Google.FirstPerson = NO -->
### Thanks
- This theme includes snippets or ideas from:
  [@SlRvb](https://github.com/SlRvb), [@Atlas](https://github.com/zcysxy),
  [@CecilaMay](https://github.com/ceciliamay),
  [@DamianKorcz](https://github.com/damiankorcz),
  [@Mara-Li](https://github.com/Mara-Li), [@kepano](https://github.com/kepano),
  [@jdanielmourao](https://github.com/jdanielmourao),
  [@deathau](https://github.com/deathau/),
  [@MelvinTing](https://github.com/tingmelvin/),
  [@EmrieCandera](https://github.com/Emrie-Candera), @lkadre,
  [@Chetachie](https://github.com/chetachiezikeuzor),
  [@pryley](https://github.com/pryley), and
  [@joelatschool](https://github.com/joelatschool).
- Many theme features are only possible thanks to the [Style Settings
  Plugin](https://obsidian.md/plugins?id=obsidian-style-settings) by
  [@mgmeyers](https://github.com/mgmeyers).
- Thanks for helping me out in my early days of learning CSS:
  [@SlRvb](https://github.com/SlRvb),
  [@javalent](https://github.com/valentine195), and
  [@NothingIsLost](https://github.com/nothingislost).

### About the developer
In my day job, I am a sociologist studying the social mechanisms underlying the
digital economy. For my PhD project, I investigate the governance of the app
economy and how software ecosystems manage the tension between innovation and
compatibility. If you are interested in this subject, feel free to get in touch.

> [!IMPORTANT]
> For questions, feature requests, or bug reports, please file an issue via 
> [GitHub](https://github.com/chrisgrieser/shimmering-focus/issues/new/choose). 
> Due to the number of messages I receive, I am not able to respond to inquiries
> made elsewhere.

- [Academic Website](https://chris-grieser.de/)
- [ResearchGate](https://www.researchgate.net/profile/Christopher-Grieser)
- [Mastodon](https://pkm.social/@pseudometa)
- [LinkedIn](https://www.linkedin.com/in/christopher-grieser-ba693b17a/)

<a href='https://ko-fi.com/Y8Y86SQ91' target='_blank'>
<img height='36' style='border:0px;height:36px;'
src='https://cdn.ko-fi.com/cdn/kofi1.png?v=3' border='0' alt='Buy Me a Coffee at
ko-fi.com' /></a>
