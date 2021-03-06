# FYProject

Latest update:

May 16, 2018 - Final update before hand-in

This update includes minor additions, revisions and improvements to the application. In addition, the project is now published as a public repository on GitHub.

You can find the repository at this address: https://github.com/d-andersen/FYProject

Furthermore, the project now also has its own website using GitHub Pages, however at the time of writing this update, the website has yet to be updated. You can find this page via the address: https://d-andersen.github.io/FYProject/


Listed below are some of the changes included in this update.

* A guide on protein synthesis has been added. The guide can be accessed via the help menu at the top or by pressing F1.

* An alternative version of the Nussinov algorithm has been added, which uses an energy function to minimize free energy in the sequence. Choosing which algorithm the application should use, can be selected in a small box, placed in extension of the sequence input area.

* The visualizations have been updated to accommodate the addition of the energy variant of the Nussinov algorithm.

* The welcome screen should now be even more welcoming, providing direct access to the main features of the application.

* Some tooltips have been added.

* The Nussinov algorithm has undergone minor revisions in an effort to fix a bug.

* Further bug hunting has squashed additional minor bugs.


*- Dennis*

---

April 22, 2018.

The project has now been updated, with the application having gone through a major rework, such that it now more closely follows the ModelViewController pattern. The impact of these changes is most evident in the `main.java` file, which has now been split into `controller.java` and `view.java`, with the result being that the application has been completely restructured. The `controller` now manages all functionality and takes care of all inputs from the user. In addition, all clickables should now have functionality attached. The `view` contains the improvements upon the original layout code.

Additional features have added as well and others improved upon. These include loading and reading of multiline FASTA files and movable visualizations; re-adding matrix and dot-bracket representations; listing of matches found and additional visual improvements.

For a better overview of the major updates of this version, see the list below:

* The entire application has been restructured to be more inline with the ModelViewController pattern.

* Added loading of multiline FASTA files. Please note that when loading FASTA files which contain sequences using the letters 'A', 'C', 'G' and 'T' the application will replace all occurrences of the letter 'T' with the letter 'U'.

* Added a result bar to the visualization area, which displays a list of the matches found. The result bar is both closable and movable. In addition, a header is shown when displaying the sequence computed. This header can be turned off.

* Readded the matrix representation to the application. The matrix representation is now shown in a movable box, which can also be closed if desired.

* Readded the dot-bracket representation to the application. The dot-bracket representation can also be turned off.

* Improvements have been made to both sequence visualization and circle visualization. These improvements include:
  * Both visualizations are now movable and zoomable.
  * Matchlines are now colored, and sized more inline with the type of binding.
  * Matchlines now overlap less often (sequence only).

TL;DR Moar update moar better! 🤘

*- Dennis*

---

April 18, 2018.

As mentioned previously, the intention is to update this `README` as the project progresses. It is also a good place to keep a changelog or ideas.

The project has been updated with the following changes:

* A file `Visualize.java` has been added, which contains the currently implemented visualization functionality. The application can currently draw the RNA string as a sequence, including matches, and as a circle representation, also including matches. However, there are some known issues:
  * When matches are drawn in the sequence visualization, lines currently overlap, which is not what is intended, so we need to look into a fix for that.
  * With the circle representation lines *occationally* overlap. As with the sequence visualization, some adjustments are needed.
* The `main.java` file has been updated to include a temporary implementation of the left toolbar, such that sequence visualization and circle visualization can be toggled on and off. This change has currently disabled the Matrix view.
* Tiny images have been added.


The repository still contain the following files:

* `Main.java` contains the runnable part of the application, so you should open this file in IntelliJ and try to run it.
* `Nussinov.java` contains the implementation of the Nussinov algorithm from the slides Philipp provided.
* `CloseBox.java`, `AboutBox.java`, `LoadTextFile.java` and `Tuple.java` are all helper classes which serve different purposes, which should hopefully be fairly clear from their titles.
* `Controller.java` and `application.fxml` currently serve no purpose. These will be needed if we wish to *style* the application later. They might also be helpful in achieving other things. Philipp might be able to elaborate on this.
* `welcome.txt` and `help.txt` both contain some filler text which is loaded into the application when needed.
* `VisualizationAttempt.java` which is a runnable version of the first attempt at implementing the visualization functionalities.

*- Dennis*

---

April 11, 2018

To my fellow students 😃

Within this repository you will find the initial upload of the application. You should clone this repository into IntelliJ. Once you have done that, we can all work on the same files "simultaneously". However, please do note that we should avoid working simultaneously on the same specific parts of the code, as this may lead to conflicts with Git - and unwanted debugging! In other words, we should coordinate 😋

The repository contains a number of files, and each file should have a decent amount of comments, which should help explain what most things do. A small description of each file is given here.

* `Main.java` contains the runnable part of the application, so you should open this file in IntelliJ and try to run it.
* `Nussinov.java` contains the implementation of the Nussinov algorithm from the slides Philipp provided.
* `CloseBox.java`, `AboutBox.java`, `LoadTextFile.java` and `Tuple.java` are all helper classes which serve different purposes, which should hopefully be fairly clear from their titles.
* `Controller.java` and `application.fxml` currently serve no purpose. These will be needed if we wish to *style* the application later. They might also be helpful in achieving other things. Philipp might be able to elaborate on this.
* `welcome.txt` and `help.txt` both contain some filler text which is loaded into the application when needed.

I think that's it for now. The intention is for this `README` to be updated along the way. How frequent however, time will have to tell. 😃

*- Dennis*
