# Corpora - Workflows for fast access to the _Thesaurus Linguae Graecae_ and the _LOEB Classical Library_  

Corpora is the plural form of corpus, a word that means denotes a large collection of writings of a specific kind or on a specific subject (American Heritage Dictionary). The ideia of this repository is to make available different workflows that I have developed while working with these corpora of text, that is, TLG and LOEB. Hopefully they will be useful to others working on themes related to antiquity.

The first release has to do with accessing the texts quickly and directly (thus shortening the time it would take for you to go online, hit the search, type, wait for results and choose a text). With these workflows, I can simply press ⌘Space (to open Alfred) and start typing whatever it is that I am looking for to see a list of possible results from the TLG and LOEB databases. After finding the entry, I can either i. hit ⌘⏎ to open the text online or ii. hit ⌃⏎ to open it offline (in case you have Diogenes installed).

There are also some functions related to a software called DEVONthink. I highly recommend checking it out. I have written about how I use it here. There is no mystery to these functions. If you hit ⇧⌘⏎ the online page with the text will be open and stored in DEVONthink and an applescript I wrote will add metadata to it (such as author name, work title, tlg code and tags). Likewise, if you hit ⇧⌃⏎ the page opened will be the offline instead.

New in Version 1.0.4: In this new version I have added the option of copying parts of the data, thus making the workflow useful for citing. If you simply hit ⏎, it will set to the clipboard the TLG code or LOEB Volume + Year. If you hit ⌥⏎, it will set the Work's Title and if you hit ⇧⌥⏎ it will set the Author's Name.

**What is next?**  
Every time I import a text to DEVONthink I need to format it according to my needs. To do so, I use several text manipulation macros which I will begin to share shortly.

**After that?**  
This will depend a lot on finding time to acquire the skills necessary to create new functions and improve old ones. This is a work in progress.

To download the workflows, go to the [releases page](https://github.com/bcdavasconcelos/Corpora/releases).

<p align="center">  
<img src="imgs/corpora1.png" width="70%" height="70%">
 </p>


## How to use it

*If you just need the workflow for quick access to TLG and LOEB, you can use either the Keyboard Maestro macro or the Alfred Workflow: it’s up to you.*

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
    * ⏎ Copy Code (TLG / LOEB Vol + Year)
    * ⌥ Work's Title to the clipboard
    * ⌘ Open Online
    * ⌃ Open Offline
    * ⇧⌥ Author's Name to the clipboard
    * ⇧⌘ Save Online link to DEVONthink
    * ⇧⌃ Save Offline link to DEVONthink
    * ⇧ Open Perseus Catalog Entry (for TLG Only)

 <p align="center">  
<img src="imgs/corpora3.png" width="70%" height="70%">
 </p>

For a demonstration, watch this [video](https://youtu.be/90hw0ER2bBQ).

## What's new?

### 2019-08-28
#### Corpora 1.0.4 for Alfred is out.
* New in Version 1.0.4: 
    * The Alfred version now is self-sufficient (i.e. it no longer relies on Keyboard Maestro) and has a few extra features.
    * In this new version I have added the option of copying parts of the data, thus making the workflow useful for citing. 
      * If you simply hit ⏎, it will set to the clipboard the TLG code or LOEB Volume + Year. 
      * If you hit ⌥⏎, it will set the Work's Title and if you hit ⇧⌥⏎ it will set the Author's Name.

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


### "I Sheet You Not" 
Source: http://www.deanishe.net/i-sheet-you-not/
This workflow was re-built using a workflow generator called "I Sheet You Not" by Dean Jackson. It greatly enhanced its ability to deal with multiple variables. Many thanks to him!

### The Perseus logo:
Source: http://www.perseus.tufts.edu/hopper/
Perseus is a non-profit enterprise, located in the Department of the Classics, Tufts University.

### The LOEB logo: 
Source: https://www.loebclassics.com/page/logo
The Logo of the Loeb Classical Library®, featuring Athena, goddess of wisdom, and Nike, goddess of victory. 

### The data
Source: https://github.com/fractaledmind/Classical-Studies-Resources
This workflow uses data collected in JSON format by Stephen Margheim, with modifications. Many thanks to him!
