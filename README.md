# Ralsei Bot Assets
Hello! These are the assets used by the Ralsei Bot, as of version 2.0. Not only is this repository available for volunteer translation, but also for some users to input their own strings! As of 2.0, Ralsei will automatically get responses from string arrays from within these asset files, which means you can add responses that you think users will benefit from, and push them onto this repository!

To get started, fork this repository, clone the fork, change the files around, push it into GitHub, and then submit a pull request. That's the basics of getting your changes into this repository.

All the strings and assets under here are licensed under the Creative Commons CC-BY-SA 3.0 License. You are free to use these in your own projects, albeit if you're trying to start a copycat Ralsei Bot using the same strings, I would definitely not appreciate that.

# Internationalization and Localization
Internationalization and localization, also known as **i18n** is the process of making a piece of software conform to multiple languages all around the world. Ralsei Bot's strings are published here in order to support this goal. If you can localize the strings used by Ralsei Bot to your language, we can make the bot more accessible to non-English speakers.

All the string sets here are labeled by their "locale string", an identifier which contains a code representing the language and another code for the location. For example, `en_US` has the language code `en` representing "English" and the location `US` representing the United States.

## Note to Translators

All internal strings are supposed to be in English - United States format.

When translating, keep in mind of the following:

### String Sets
Per language, there are usually four string sets.
* **Boxes** - Box responses written in box syntax. This file should contain nothing but box syntax.
* **Commands** - Command metadata, namely display names and descriptions. It should also contain metadata translations.
* **Config** - Strings used for configuration, which usually includes descriptions of commands or command usages, along with responses.
* **Embeds** - Contents of MessageEmbeds.
* **Meta** - Translatable parts of the bot meta. This includes the bot name. For example, "Ralsei Bot" in Japanese (ja_JP) becomes "「ラルセイボット」". If untranslatable (or the meaning will be extremely lost in translation), it is left as is.

### Commands
The following are to be localized:
* Command display names
* Command triggers
* Attributes (flags)

The following are **NOT** to be localized:
* **Names** - They are internally used and should not be localized.
* Specifically the following command triggers:
    * `configuration`
    
Additional notes:

* Most command triggers are only one word long. Therefore, triggers can only match the first word.
* When modifying command triggers, make sure that it will still match the English versions.

### Embed Content
Embed descriptions, footers, headers, etc. should be localized.

### Configurations
Configuration keywords must not be localized. However, configuration resposnes, descriptions and the like should be.

Also, leave the `displayName` field alone.