# Corpora - Workflows for fast access to the _Thesaurus Linguae Graecae_ and the _LOEB Classical Library_  

**Corpora** has two different workflows on different softwares in order to access TLG and LOEB.  
Both this softwares, namely, [Alfred](https://www.alfredapp.com) and [Keyboard Maestro](https://www.keyboardmaestro.com), are highly recommended. You can use either one of them.  
_**Only if**_ you need integration with [DEVONthink 3](https://www.devontechnologies.com/apps/devonthink), then you necessarely need the Keyboard Maestro macros. For DEVONthink, **Corpora** has an applescript to set _Author Name_, _Work Title_, _TLG Code or LOEB Link_ and _tags_ automatically.  

## How to use it

Again: **If you just need the workflow for quick access to TLG and LOEB, you can use either the Keyboard Maestro macro or the Alfred Workflow: it’s up to you.**
**For integration with DEVONthink, you’ll need to install the Keyboard Maestro macros.**

### On Keyboard Maestro
* Import the library and make sure it is enabled.
* Follow the instructions on the macro on how to set it up properly: you’ll need to provide the path to the folder where the LOEB offline files are (in case you intend to use it), and the path to the folders where you want the records to be created and stored on DEVONthink (in case you are using this software as well).
* Trigger the macro with the choosen shortcut.
* You'll see a prompt for authors and works containning both TLG and LOEB Classical Library volumes. 
* Enter search term, then using the arrows, select one and press return.
* Choose whether you want this link to open online or offline.
* Choosse whether you want to open this link on the default browser or store it on DEVONthink 3.
* You'll be taken directly to the text.

### On Alfred
* Type _z_ and _space_ (You can edit the keyword to activate the workflow as you please)
* Enter search term. Using the arrows, select one.
* You can see and choose alternative options by pressing ⇧, ⌘ and ⌥.
	* By pressing ⏎ you’ll open the text on TLG/LOEB online on your deafult browser.
	* By pressing ⌘⏎ you’ll save the reference to DEVONthink.
	* By pressing ⇧⏎ you’ ll open offline version.
	* By pressing ⌥⏎ you’ll save the reference of the offline version to DEVONthink.

For a demonstration, watch this [video](https://youtu.be/90hw0ER2bBQ).

## What's new?

### 2019-08-19
* **Corpora** now has its own repository and two different workflows on different softwares.
* A new [**Alfred**](https://www.alfredapp.com) workflow was created with the capability of accessing TLG and LOEB online and offline.
* For a integration with DEVONthink the workflow still relies on Keyboard Maestro.
* In order to make this integration possible, the main macro was divided into several smaller units, so on Keyboard Maestro it now appears as a macro library instead of a single macro.
* **A search bar can be launched both from Alfred and Keyboard Maestro.**

### 2019-08-14 

* A brand new macro was created and a lot of work was put into this. Both macros (TLG Macro and LOEB Macro) are now united and working perfectly in alfred-style.

<p align="center">  
<img src="https://github.com/bcdavasconcelos/mykmmlibrary/blob/master/Screenshots/corpora.png" alt="Prompt for Author or Work" width="70%" height="70%">
 </p>  

* Dependencies on third party plug-ins were eliminated!

* DT3: Author and work names, TLG code and tags are set automatically via Applescript. This relies on a new Keyboard Maestro 9.0 feature for JSON dictionaries.


> The macro use data collected by @fractaledmind ([Stephen Margheim](https://github.com/fractaledmind/Classical-Studies-Resources)) in JSON format, with modifications.
