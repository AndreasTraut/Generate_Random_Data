Author: Andreas Traut  
Date: 29.06.2020  
[Download as PDF](https://github.com/AndreasTraut/Generate_Random_Data/raw/master/Generate%20Data%20Installation%20Steps%20for%20Beginners.pdf)  

# Installation steps for “Generate Data”

# Purpose of the application “Generate Data” and limitations

I found the tool “Generate Data” (<http://www.generatedata.com/>), which
is available for free (Open-Source on GitHub). Whith “Generate Data” you
are able to generate randomized data according to user-specific rules.
Defining the user-specific rules can be done in the following formula.
Unfortunately this is restricted to maximum 100 rows:

![](./media/image1.png)

You can define the columns and data types as shown below, e.g. I want
“*myname*” to be a non-gender-specific name, “*myemail*” to be an
E-Mail address, “*myspecialnumber*” a number according to a special
format (e.g. “LLL-Xxx-L” which I will explain later), “*myregion*” to be
region in Germany (e.g. “Bayern”, “Rheinland-Pfalz”,…). These
definitions look like shown below:

![](./media/image2.png)

After having pressed “Generate” an Excel will open, which contains 100
rows of randomized data according to the user-specific requirements,
which we defined above, e.g. the Excel-Sheet as shown below:

![](./media/image3.png)

The limitation of the browser version of “Generate Data” as described
above is, that you can only generate maximum 100 rows of data. If you
need more, then you would need to install “Generate Data” on your
computer. It is free as the source code is “Open-Source” and available
in Github (see https://github.com/benkeen/generatedata). But the
installation is not easy for beginners. If you are not familiar with
MySQL and PHP, then even the official installation guide, which is
available “Generate Data” website, won’t be helpful for you (Sorry….).

# Official Installation Guide of “Generate data”

According to the official documentation on

<http://benkeen.github.io/generatedata/install.html>

you need to follow

“**Step 1: manual labour**” (which is downloading a zip file and the
setup of MySQL and PHP) and

“**Step 2: Installation script**” (which is the creation of a new
database, which is necessary for running the “generatedata”-script).

![](./media/image4.png)

I read in comments that some users were struggling in completing these
steps (me included initially, but as I describe here it is also possible
to install it for absolute novices). I want to close the documentation
gap between “**Step 1**” and “**Step 2**” and make the tool “Generate
Data” available also for beginners.

# My installation guide 

First you need to install “**XAMPP**” (the database and PHP). Therefore
go to website

<https://www.apachefriends.org/index.html>

and download the XAMPP file (e.g. for Windows, see red circle):

![](./media/image5.png)

Follow the installation process. When you are asked for choosing an
installation folder, then choose

**C:\\xampp\\**

as the installation folder.

You may select only „**Apache**“, “**MySQL**” and „**PHP**“ only and
unselect the other options (e.g. you don’t need Pearl, FileZilla,
Mercury, Tomcat…).

Then goto C:\\xampp\\ and start the application “**XAMPP Control
Panel**”, which is the file called

**xampp-control.exe**

You will see the following screen. Start “**Apache**” and “**MySQL”** by
pressing the marked buttons:

![](./media/image6.png)

When Apache and MySQL have been started it will look like this:

![](./media/image7.png)

Then open a browser (e.g. Firefox-Browser) and type:

**localhost**

into the browser search window as shown in the screenshot below (red
arrow). If everything was successful the welcome “**Dashboard**” of
XAMPP will open:

![](./media/image8.png)

Now open the installation page for “**generaldata**” which is this one:

<http://benkeen.github.io/generatedata/install.html>

and download the latest version (the **ZIP-file**) as shown in the
screeshot below (see red arrow):

![](./media/image9.png)

Extract the ZIP-File and put it into the **xampp** Folder -\> Subfolder
“**htdocs**”. For example, if your installation folder in the
beginning has been **C:\\xampp** as I suggested to do, then put the
extracted zip-content of “generatedata” into

**C:\\xampp\\htdocs\\**

as shown in the screenshot below:

![](./media/image10.png)

Now open your browser and type

**localhost/generatedata**

as shown in the screenshot below:

![](./media/image11.png)

The installation Window for “generatedata” should open as follows:

![](./media/image12.png)

Congratulations: if you see this window above, then you already
completed the first three tasks (“Step 1”) of the official installation
guide, which are described here:

<http://benkeen.github.io/generatedata/install.html>

![](./media/image13.png)

Next would be to complete “**Step 2: Installation Script**”. But before
you can do this you need first to create a database and user for it. How
can this be done? Well, we need to open the “**phpMyAdmin**” site as
follows: go back to the "**XAMPP control panel**" (see above) and press
“**Admin**” as shown in this screenshot (alternatively you can also
type “**localhost/phpmyadmin**” into the search window in your browser):

![](./media/image14.png)

Your browser (e.g. Firefox-Browser) will open. This is the
**pypMyAdmin** Page. Goto 1 “**Databases**” and then create a new
database (2 and 3) as follows:

![](./media/image15.png)

After having done this you will see you new database as follows (see red
arrow):

![](./media/image16.png)

Now we need a new user. Therefore goto 1 “**Useraccounts**” and then 2
“**Add user account**” as shown here:

![](./media/image17.png)

As shown in the screenshot below, define 1 “**User name**”,
“**Password**” and then select 2 “**Global privileges: check all**”
(this manual is for beginners, and it is easiest to grant all
privileges. Later you can come back to this point and limit the access
rights a bit, which in my opinion is not necessary: we are not dealing
with an encrypted back software here). Then press 3 “**Go**”.

![](./media/image18.png)

After having created a new user you will see it as shown here (later:
click “**Edit privileges**” for changing privileges):

![](./media/image19.png)

Now open the browser (e.g. Firefox-Browser) and type

**localhost/generatedata**

and you will be able to continue the official installation steps “**Step
2: Installation script**” as described in the manual

<http://benkeen.github.io/generatedata/install.html>

I will show below how this looks like below.

![](./media/image13.png)

Enter the **database name**, **username** and **password**, which you
created above. Press “**Continue**”.

![](./media/image20.png)

Next press “**Create file**”:

![](./media/image21.png)

Next select “**continue**”:

![](./media/image22.png)

Then press “**Install Plugins**”:

![](./media/image23.png)

You can select all plugins. Only if you know for sure, that you don‘t
need all you can deselect some (which I don’t recommend). Press
“**Continue**”.

![](./media/image24.png)

Then press “**Go to script**”:

![](./media/image25.png)

**The installation is finished\! Congratulations\!**

You will see the following window and you are ready to create your
datasets. Define a name (e.g. “**mydataset**”) and country-specific data
(e.g. “**Germany**”):

![](./media/image26.png)

Next you can define “**Column titles**“ and “**Data type**“ (see 1). If
you want specific options, then use the “**?**” button (see 2).

Select 3 “**Excel**” and 4 “**250 rows**” and then press 5
“**Generate**”.

![](./media/image27.png)

When you press the button 2 “**?**” (the question mark) the window below
will open and explain the various options. For example “L” is an
uppercase Letter and “x” / “X” are numbers. I defined “**LLL-Xxxx-L**”
as my special format (see above):

![](./media/image28.png)

After having pressed the 5 “**Generate**” button, an Excel file will
open. In my case it looks like the one below:

![](./media/image3.png)

If you need this format more frequently you can save it for being use
later again. Press 1 “**Save**”. Use button 2 to load saved datasets:

![](./media/image29.png)

Obviously the names above (e.g. “Stephen”, “Matthew”,…) must be saved
somewhere. Yes, exactly: they are saved your database (mine was
“**mydatabase**”, see 1 in the screenshot below). You can open the
according database-table by going to the **phpMyAdmin** site (have a
look in my documentation above, if you don’t remember how this can be
done). Then goto 2 “**gd\_first\_names**”. As you can see you can 3
“**Empty**” the table and 4 “**Insert**” new names:

![](./media/image30.png)

I think if you reached this point, then you should be fine for
progressing yourself.

I hope this helped a bit some people, who are not too familiar with
MySQL or PHP and want to run “Generate Data” on their own personal
computers without limitations.

Greetings  
Andreas
