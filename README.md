# Sharepoint Versions & Applicability
At time of writing this repo the version & date was
Menus & actions may move around within sharepoint as microsoft updates sharepoint but you should be able to find them if you search for them.

# Background to this repository
I was asked to help out with a wiki development team which had the content to put on the page but it was all very wordy with no clear layout and very hard to navigate. This repository was my answer. Although it is very custom and specic to the task at hand I though the code and the approach I took to echieve this would be helpful to others.

# CustomSharepointSite
This repository holds code used to create a custom wiki site on Sharepoint built with HTML/CSS.
Firstly you need to create a sharepoint site & create a new blank wiki page for your first page (this is assumed that you will know how to do and wont be covered in this repository read me).

# Removing the Top & Side menus provided by sharepoint (this is to allow you to create/use your own navigation menu - less confusion for your sharepoint wiki users)
To do this you need to first create a space to allow custom code which will remove these menus.
(From a blank wiki page within sharepoint) go to: 
Edit > Insert > Web Part > Media & Content > Script Editor > Add
Once the script editor has been added select the editor > Using the drop down arrow in the top right of the editor window > Edit Webpart > Edit Snippet > Then copy & paste the following code:
<style>
#sideNavBox { DISPLAY: none }
#contentBox { margin-left: 0px }
#titleAreaBox { DISPLAY: none }
</style>

# Now that the standard sharepoint navigation menu's are gone we can focus on building our own web page with intenral navigation links.
