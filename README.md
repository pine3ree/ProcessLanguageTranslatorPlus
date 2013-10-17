Process Language Translator Plus
===========================

- Version 1.0.0
- Release State: alpha
- requires: ProcessLanguageTranslator

Same like Language Translator Modul. You will get a drop-down list to select translatable files instead of text field.  
path: admin/setup/language-translator/add/


### How to Install:
- load up module to directory: wire/modules/LanguageSupport/
- go to: pages -> admin -> setup -> language-translator -> edit -> process
- choose: 'ProcessLanguageTranslatorPlus' from the list and save
- Done!

### Roadmap:
Implement Switcher to select another Language in the Translator

##### current-settings:
If language specified as a GET var in the URL, the Module will pick it up and use it (will be stored in session),
else if there exists a session var (translateLanguageID) this will be used,
else as default-setting the language of logged-in user will be used

##### change Language with GET Parameter like:
admin/setup/language-translator/add/?language_id=1022

language_id should be a valid language->id on your system.



