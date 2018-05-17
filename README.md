# Collaboration with Google Apps Script Example
Example for Learning Git with Apps Script

This exercise is meant to help you learn how to collaborate using Google Apps Script.
In particular, we will be using the tools [GitHub](https://guides.github.com/activities/hello-world/)
and [Clasp](https://codelabs.developers.google.com/codelabs/clasp/#0).

I assume you know what a terminal is and are familiar with simple commands such
as `cd`, `ls`, etc.

For Git, you should learn what the following commands are:
* `git clone`: for downloading a repository on GitHub to your own machine
* `git add`: when you have new files that you need to track (the --all flag is helpful, too)
* `git commit`: to tell git that you have changes you want to update (the -a and -m flags are useful)
* `git pull`: do this before you push to make sure you have the most recent code from GitHub
* `git push`: do this to send your commit to GitHub for everyone to see
* `git status`: good for keeping track of your files and in case you have errors

For Clasp, you should install it by doing the following:
* [Install Node](https://nodejs.org/en/download/) if you do not have it on your computer.
* Install Clasp by running `sudo npm i @google/clasp -g --unsafe-perm` which may ask for your computer's password
* Verify that you have successfully installed Clasp by running `clasp` and seeing a list of options appear

Next you'll want to login to Clasp by running `clasp login` which will open your
web browser and allow you to pick a Google account. If you ever want to change
accounts, just run `clasp logout` and login again.

Now, go ahead and clone this repository to a convenient directory on your computer.
I recommend keeping a directory called HAUSCRtech in a easy-to-find place. After
cloning the repository, you should see a bunch of files, which you can list with
the `ls` command. If you `cd` into the `Code` directory, and then run `clasp open`,
your browser should take you to the Google Script editor where you will see some code.
Close this for now, since *you should avoid having this open while editing locally*.
Edit the file `Code.js` inside the `Code` directory by adding a line that inserts
your name into the spreadsheet at the cell below the most recent person to edit the
code. Then, run `clasp push`, which takes your local code and puts it on the Google 
Script editor. You can then run `clasp open` and click the Play button to actually
run the code. The result is visible in [this spreadsheet](https://docs.google.com/spreadsheets/d/1M-3v2b4eGb736QOrQ1AY6pcC8lQJkqyy9vAXK2Wjn9w/edit#gid=0). Note that running
`clasp push` is not sufficient for collaborative development. If you are happy
with your results and do not have errors, you should commit and push your changes
to GitHub so that we update the central repository we are all using.

I strongly recommend looking at [this codelab](https://codelabs.developers.google.com/codelabs/clasp) for more practice with Clasp!
