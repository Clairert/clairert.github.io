---
layout: page
title: Project Two Blog
---
## Project Two

### Week One
I began taking stock of where the project was left off from last semester. I made a list of objectives for the next two weeks before meeting with David. The main ideas were:
* Researching strategies to raise awareness of the gazetoolbar.
* Finishing some left over code clean-up for the toolbar.
* Initial reasearch into adding environmental controls to the toolbar.

I created an new email address for the project and added the contact information to the accessibility software website. I also used the email address to create a new reddit account. I made a list of subreddits that I believe would be a good place to advertise the toolbar and saved them to the account to be approved of at a later date.

### Week Two
I have removed unnecessary code from the settings page and moved around the panels to make it easier to figure out where all the panels are. I have also removed all references to the microphone as that functionality has been removed. I left in the dynamic zoom buttons for now as I intend to fix them and re-enable funtionality there.

I have written a draft for the posts on reddit. It still needs to be edited and approved but it has been started. 
I have begun to re-implement the previous version of dynamic zoom so I can edit it as planned. I changed the default settings to turn on dynamic zoom temporarily as the buttons are not on the settings page at the moment. Sadly the previous version of dynamic zoonm is not working. I have begun troubleshooting to find the source of the error as visual studio is not telling me where the error is occurring.

### Week Three

I have used Gray's branch of the project to find a version of dynamic zoom that is working and compared it to my version of the magnifier class. I located the issue as some code had been changed and have reverted it. This means that the old version of dynamic zoom is working again and I can start modifying it.

I have managed to edit the code so now the zoom window will open on one of the four quarters of the screen depending on where you are looking. While working on this I have run into an issue with the current documentation. Some of the entries on the wiki are not very detailed. They give a brief overview of the class but no clear details on how each method works and how the class itself functions. This means when I asm trying to change something I have to go through the whole class to find the method I need to change and then slowly work out what variables actually control each aspect. This has slowed me down as a whole because I am spending too much time trying to figure out how it works instead of actually changing or writing code.

I spoke to Adon about the settings page and the issues I have had with it. He agreed that the current method of opening the settings page and closing on start-up is incorrect and needs to be corrected. He advised that the current code, where the settings are being edited through the form is bad and the form should just be used to control the form. I hadn't really noticed that before as I had actively avoided the settings page before but he is correct that it was bad form of the team who made the settings page. To correct this I have begun making a seperate settings class that will contain all the acutal processing of settings and will leave the form to only handle the user input. This should allow for settings to be loaded without opening the settings page and is just better coding in general.

Updated contact page after discussing with David what needed to be changed. Also made a minor spelling correction on the credit page of the assessibility hub website.

I have deleted some of the obsolete branches off the github repository. I went through and deleted all branches that hadn't been updated in two or more years.

I have begun moving the settings into a seperate class. The settings now load on start-up from the seperate class instead of the settingsJSON class.


### Week Four

I have finished changing the code on the magnification class to open the magnification window in the corners instead of the center. Now I need to make it optional between the different settings instead of having it hard coded into the code as I have done so far for testing. This will also mean that I am going to have to edit the code for the settings page. But I might wait untill I have cleaned up my code more and finished seperating the setting json code from the form.




### Week Seven
I have replied to an email reporting a bug and have begun advertising on reddit for the toolbar.
We have discovered there is an issue with displaying the settings page on laptops. I will begin investigating this soon and hope to have it fixed before the next release at the end of the year.

Currently my plan is as follows:
* I am going to fix the zoom class architecture to be split ---->Done
* Add the zoom styles to the settings Page   ----->Done
* Change the keyboard class to allow for easy addition of adding new keyboards --->Have written the new keyboards into files. need to implement
* Create new keyboard form
* Edit form to include autocorrect
* Add in speach<--> text functionality.