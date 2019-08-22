# Corpora - Workflows for fast access to the _Thesaurus Linguae Graecae_ and the _LOEB Classical Library_  

*Corpora* is the plural form of *corpus*, a word that according to the American Heritage dictionary, means *"a large collection of writings of a specific kind or on a specific subject"*. The ideia of this repository is to make available different workflows that I have developed while working with these *corpora* of text, that is, TLG and LOEB. Hopefully they will be useful to others working on themes related to antiquity.

The first release has to do with accessing the texts quickly and directly (no more waiting for pages to load, opening the search online and so on). With them I can simply press ⌘ Space to see a complete list of the contents of these *corpora*. I will select one of them and it will automatically take me to the text that I want to see. If you happen to use Diogenes, all you have to do is press ⇧⏎ and you will open the text taken from your Diogenes data base on your browser (and the same applies for LOEB). There are some other funciontions related to DEVONthink 3, but there is mystery to them. Simply press ⌘⏎ to open and save the link on DT3. A applescript will copy part of the relevant metadata automatically. 

To download the workflows, go to the [releases page](https://github.com/bcdavasconcelos/Corpora/releases).

<p align="center">  
<img src="imgs/corpora1.png" width="70%" height="70%">
 </p>


## How to use it

*If you just need the workflow for quick access to TLG and LOEB, you can use either the Keyboard Maestro macro or the Alfred Workflow: it’s up to you.*
*For integration with DEVONthink, you’ll need to install the Keyboard Maestro macros.*

### On Keyboard Maestro
* Import the library and make sure the macros are enabled.
* Follow the instructions on the macro on how to set it up properly: you’ll need to provide the path to the folder where the LOEB offline files are (in case you intend to use it), and the path to the folders where you want the records to be created and stored on DEVONthink, in case you are using this software as well. These are the *x-devonthink...* links.
* Trigger the macro with the chosen shortcut.
* You'll see a prompt for authors and works containing both TLG and LOEB Classical Library volumes. 
* Enter search term, then using the arrows, select one and press return.
* Choose whether you want this link to open online or offline.
* Choose whether you want to open this link on the default browser or store it on DEVONthink 3.
* You'll be taken directly to the text.

<p align="center">  
<img src="imgs/corpora2.png" width="70%" height="70%">
 </p>


### On Alfred
* Type _z_ and _space_ (You can edit the keyword to activate the workflow as you please)
* Enter search term. Using the arrows, select one.
* You can see and choose alternative options by pressing ⇧, ⌘ and ⌥.
	* By pressing ⏎ you’ll open the text on TLG/LOEB online on your default browser.
	* By pressing ⌘⏎ you’ll save the reference to DEVONthink.
	* By pressing ⇧⏎ you’ll open offline version.
	* By pressing ⌥⏎ you’ll save the reference of the offline version to DEVONthink.

 <p align="center">  
<img src="imgs/corpora3.png" width="70%" height="70%">
 </p>

For a demonstration, watch this [video](https://youtu.be/90hw0ER2bBQ).

## What's new?

### 2019-08-19
* **Corpora** now has its own repository and two different workflows on different software.
* A new [**Alfred**](https://www.alfredapp.com) workflow was created with the capability of accessing TLG and LOEB online and offline.
* For an integration with DEVONthink the workflow still relies on Keyboard Maestro.
* In order to make this integration possible, the main macro was divided into several smaller units, so on Keyboard Maestro it now appears as a macro library instead of a single macro.
* **A search bar can be launched both from Alfred and Keyboard Maestro.**

### 2019-08-14 

* A brand-new macro was created, and a lot of work was put into this. Both macros (TLG Macro and LOEB Macro) are now united and working perfectly in Alfred-style.

<p align="center">  
<img src="imgs/corpora.png" width="70%" height="70%">
 </p>

* Dependencies on third party plug-ins were eliminated!

* DT3: Author and work names, TLG code and tags are set automatically via Applescript. This relies on a new Keyboard Maestro 9.0 feature for JSON dictionaries.


> The macro use data collected by @fractaledmind ([Stephen Margheim](https://github.com/fractaledmind/Classical-Studies-Resources)) in JSON format, with modifications.
