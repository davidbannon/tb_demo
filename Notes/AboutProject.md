<underline>About this Project</underline>
===========



This project is in its very early stage but maybe it will look something like this-



**Background**
--------
tomboy-ng, https://github.com/tomboy-notes/tomboy-ng is a complete rewrite of the original Tomboy Notes. Both have a sync capability, tomboy-ng currently only syncs at a file level but Tomboy could talk to various network servers. I have been reluctant to duplicate Tomboy's network model because I have some reservations about how it works, allowing some errors to happen. Further the Tomboy network sync relied on OAuth1.



That network sync did allow us to bring in Android devices using Tomdroid, tomboy-ng does have a connection to Tomdroid but it is kind of clumsy.



A solution for tomboy-ng would, IMHO, avoid the end user having to run their own network servers (with all the associated security and technical issues) and should allow people to view and edit their notes in a more modern, on line manner. But not turn tomboy-ng into a purely on-line application. And, yes, I am old fashioned enough to still want to ensure a level of privacy.



**The New Proposal**
--------
If the user is not providing their own server, then we have to use an existing one, ideally free and one that provides a reasonable level of security and privacy. I have chosen to use Github (and expect to be able to extend its operation to Gitlab). The user will be able to upload and download notes to Github as either encrypted or markdown. Markdown notes can be viewed and even edited using Github's built in editor. Notes that contain content that you consider sensitive will be uploaded, stored and downloaded again in a reasonably secure encrypted format.



By adding notes to certain Notebooks, you declare the level of privacy you require, you can further decide to treat all notes as encrypted or all as view/edit capable.



I still consider that the main use of your notes will be using tomboy-ng on a Windows, Linux or MacOS machine. But being able to sync over the network is a valuable addition, being able to view and occasionally edit, using markdown is a bonus.



**The costs**
--------
* This model will not support Tomdroid but Tomdroid has not been maintained for many years now.

* You will require a Github account. Github accounts are free and the particular repository should be marked as private (unlike this demo one). Authentication can be done in a number of ways, I have been using their token model, you generate a token on line, paste it into tomboy-ng and its good for, typically, a month.

* Accessing encrypted notes and safely storing the github token will require a password when you first start tomboy-ng. I suggest a good password policy but how careful you wish to be is up to you.



**Feedback**
--------
As mentioned, this project is very early on. If you would like to comment, make suggestions, offer advice, please do so via the tomboy-ng issues facility. https://github.com/tomboy-notes/tomboy-ng/issues








