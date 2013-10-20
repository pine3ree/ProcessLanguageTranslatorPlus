Process Language Translator Plus
===========================

- Version 1.0.0
- Release State: beta
- requires: ProcessLanguageTranslator

Same like Language Translator Modul. You will get a drop-down list to select translatable files instead of text field.  
path: [/admin/setup/language-translator/add/](#)


### How to Install:
- load up module to directory: wire/modules/LanguageSupport/
- go to: pages -> admin -> setup -> language-translator -> edit -> process
- choose: 'ProcessLanguageTranslatorPlus' from the list and save
- Done!
- Do not uninstall the original ProcessLanguageTranslator in the Module settings, it is required!

### Settings (developers info):
- If language specified as a GET var in the URL, the Module will pick it up and use it (will be stored in session),
- else if there exists a session var (translateLanguageID) this will be used,
- else as default-setting the language of logged-in user will be used.  
  change Language with GET Parameter like:  
  admin/setup/language-translator/add/?language_id=1022  

### Use:
If you are in the Language Translator [/admin/setup/language-translator/](#) you can see a List of Files which are already translated (in the set language).    
Click Button "Translate New File" to reach the Translate File Selector [/admin/setup/language-translator/add](#).  
Select a not yet translated file from the list.  
Click the Button below to create a translation file and go directly to the Editor.  
Via the Language-Switcher you can easily switch to the Translator of another Language. 

![Module Screenshot](http://processwire.com/talk/index.php?app=core&module=attach&section=attach&attach_rel_module=post&attach_id=1818)

### Roadmap:
- providing a Button in the Language Translator to download a zipped Language-Pack created from the current Edition. 
- output of further Information (translation files without original, duplikates)
