# Introduction 
This project is trying to solve the issue of not having multiple languages to choose from in different regions and their dedicated game client. If you just copy over the files from another regions game client, there will be missing translations all over.

It initially started with making the translations from the international game client available for the Japanese game client as well, but it already expanded beyond that and provides ready-to-use translations for `iToS` (International), `jToS` (Japanese), `twToS` (Taiwanese). Translations for `kToS` are in the works.

Here is an overview of all the supported languages
||iToS|jToS|twToS|kToS
|---|---|---|---|---|
|English|〇|〇|〇|
|German|〇|〇|〇|
|Portuguese|〇|〇|〇|
|Russian|〇|〇|〇|
|Indonesian|〇|〇|〇|
|Thai|〇|〇|〇|
|Chinese|〇|〇|〇|
|Taiwanese|〇|〇|〇|
|Japanese|〇|〇|〇|
|Korean|〇|〇|〇|

Having all these languages is achieved by using translation files of two selected builds and get them mapped programmatically by comparing their original Korean texts. 
This method is not free of mistakes and might end up not translating some texts at all but gives an overall good result to play the game comfortably with in your desired region!


# Installation
Open the according folder of the game client you want to use the translations with, either `iToS`, `jToS` or `twToS`.
Then move the language folders (e.g. `English`) in the games `languageData` folder.

One languages folder path should then look something like this:
```
../Steam/steamapps/common/Tree of Savior (Japanese Ver.)/release/languageData/English
```
Do this with all the languages you want make available in-game and you're ready to go!

# FAQs
### Translations cause display issues with some CJK characters. What can I do?
This might be caused due to the game being launched with the wrong localization. In case of the Japanese game client, it should always be launched with Japanaese localization, either by setting it in your OS or using a tool *(e.g. Locale Emulator)* to execute the application in said localization. This applies to other CJK clients as well.

### Some texts are not translated or display just what seems to be an ID, why?
Due to the translations being mapped programmatically they will not be free of error and any hint towards missing or faulty translations is always appreciacted!

# Contribute
If you find any mistakes or missing translations that are available already or you know the translation of, feel free to open up an issue or a pull request!