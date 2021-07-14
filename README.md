![Website](https://img.shields.io/website?url=https%3A%2F%2Ffindadocjp.org%2F)
[![ESLint](https://github.com/ourjapanlife/findadoc-localization/actions/workflows/eslint.yml/badge.svg)](https://github.com/ourjapanlife/findadoc-localization/actions/workflows/eslint.yml)
[![Python application](https://github.com/ourjapanlife/findadoc-localization/actions/workflows/python-app.yml/badge.svg)](https://github.com/ourjapanlife/findadoc-localization/actions/workflows/python-app.yml)
![GitHub](https://img.shields.io/github/license/ourjapanlife/findadoc-localization)
![Forks](https://img.shields.io/github/forks/ourjapanlife/findadoc-localization?label=Fork)

# Find a Doc - Localization

[Join our Slack!](https://join.slack.com/t/find-a-doc/shared_invite/zt-s4744a6o-MGaGHzLN5wB9aXeha3vdsQ)

[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/theyokohamalife)  

[Find a Doc](https://findadoc.jp) is a free online resource aimed at helping connect the foreign community in Japan with health services in their native language.

Translations are initially created by machine in a special file format, and then edited by volunteers to be published on the site.

## How to Contribute

If you speak a foreign language and can help translate files, Go to 👉️ [Translator Guide](#translator-guide)

If are a developer trying to add internationalization (i18n) keys, Go to 👉️ [Developer Guide](#developer-guide)


## Translator Guide

The easiest and fastest way to contribute our project is through our page on Github (a platform for open-source coding projects). Simply **clone this repo and open a PR to merge your changes**.

If you're new to Github, here are some easy steps you can take to get started:

### Beginner Github

1. Go into the [locales] folder (https://github.com/ourjapanlife/findadoc-localization/tree/main/locales) and click on the language file you wish to contribute to. It will take you to a screen that will show you its content. 
2a. If you are creating a new language file, copy from `en.json` and please name the new file using the two-letter language codes defined [here](https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes))
   ![Select Language](./images/01.png)
   ![Select Language](./images/01.1.png)

2b. If you are editing an existing file, click the `edit` button (box with a pencil in the upper right corner of the page). Then you can directly edit the translation through your browser. **Use the `en.json` file and the [website](https://findadoc.jp) as the reference content.**
   ![Edit Button](./images/02.png)
   
   
_Make sure to only edit the words inside of the quotation marks of your selected language._

You might notice the files are in a special format so the computer can read it. This format is called JSON (JavaScript Object Notation) and contains
a key on the left side, and a value on the right side. Notice that the key names are in English, and sometimes the letters are squished together like this `noSpacesHere`. Please only edit the values, not the keys. Note the example below has a key of "vaccine" and a value translated into Japanese.
```json
{
   "key": "value",
   "vaccine": "ワクチン"
}
```

If this is confusing or you get stuck, we are here to help. See contact information below 😊

3. Select the `Create a new branch for this commit and start a pull request` option at the bottom of the page. Then click the `Propose changes` button.
   ![Create Branch](./images/03.png)

4. Optional - Add any comments you want to make on the pull request screen.
   ![Open PR](./images/04.png)

5. Click the `Create pull request` button.

Thank you! Your changes will be reviewed!

_If you have any trouble with this document, please file an issue or reach out to [@stonecoldkilzer on Twitter](https://twitter.com/stonecoldkilzer)_

## Developer Guide

1. Fork & clone this repo to your computer
2. Edit the `locales/en.json` to contain the new keys.
3. If you know another language, feel free to add the same key and translation to the appropriate locale file. Omit if you don't know it; we use English as the [fallback language](https://kazupon.github.io/vue-i18n/guide/fallback.html) so nothing will break.
4. Make a pull request in this repo and wait for it to be merged to `main`
5. Make your change in the [parent repository](https://github.com/ourjapanlife/findadoc-frontend) with the new i18n keys and submit your PR 🎉
