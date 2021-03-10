# MacOS Terminal Protected Zip Guide

This is a super quick guide for zipping a directory with password protection using MacOS Terminal.


**PREP YOUR FILES:**

First off, prepare your directory and it's files somewhere that's easy enough to get to via Terminal.

> We'll work through this assuming there's a directory located in the Desktop directory called `my-files`, that contains three image files named `1.jpg`, `2.jpg`, `3.jpg`.


**LAUNCH AND NAVIGATE IN TERMINAL:**

Next, fire up Terminal and navigate to (in this example) the Desktop directory with:

```bash
cd Desktop
```

You could double check that the directory you want to zip and protect is there in Terminal (in our case one called `my-files`) with:

```bash
ls
```

The above command (in our case `my-files`) should show your directory to zip for the next step!


**Run Your Zip Command:**

```bash
zip -er my-files.zip my-files/
```


**Set Zip Password:**

The command above will trigger Terminal to ask you to type or paste in a password (twice) before saving your file. It's makes things easy to plan out your password and zip file command before even getting into Terminal, so you can quickly and confidently create your file and store or distribute as needed with peace-of-mind that the .zip's contents are a bit more secure in transit.

> **NOTE:** These files will trigger warnings in email services like Google's Gmail, because they cannot be auto-scanned for viruses. So communicate this detail proactively whenever sending out protected zip files made using this Terminal technique!
> 
