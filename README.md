# MacOS Terminal Protected Zip Guide

This is a super quick guide for zipping a directory with password protection using MacOS Terminal.


---

## Table of Contents

* [Prep Your Files](#prep-your-files)
* [Launch and Navigate in Terminal](#launch-and-navigate-in-terminal)
* [Run Your Zip Command](#run-your-zip-command)
* [Set Your Zip's Password](#set-your-zips-password)


---


### Prep Your Files:

First off, prepare your directory and it's files somewhere that's easy enough to get to via Terminal.

> We'll work through this assuming there's a directory located in the Desktop directory called `my-files`, that contains three image files named `1.jpg`, `2.jpg`, `3.jpg`.


---


### Launch and Navigate in Terminal:

Next, fire up Terminal and navigate to (in this example) the Desktop directory with:

```bash
cd Desktop
```

You could double check that the directory you want to zip and protect is there in Terminal (in our case one called `my-files`) with:

```bash
ls
```

The above command (in our case `my-files`) should show your directory to zip for the next step!


---


### Run Your Zip Command:

Next, you want to get your zip file command to work it's magic. To do this, you'll want to use the `-er` flag(s), specify the name of your new .zip file, then add a space, and finally specify which directory you intend to archive into your new .zip filename like so:

```bash
zip -er my-files.zip my-files/
```

---


### Set Your Zip's Password:

The command above will trigger Terminal to ask you to type or paste in a password (twice) before saving your file.

It's makes things easy to plan out your password and zip file command before even getting into Terminal, so you can quickly and confidently create your file and store or distribute as needed with peace-of-mind that the .zip's contents are a bit more secure in transit.

> **NOTE:** These files will trigger warnings in email services like Google's Gmail, because they cannot be auto-scanned for viruses. So communicate this detail proactively whenever sending out protected zip files made using this Terminal technique!
> 
