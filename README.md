# `allcommands.io`
> allcommands.io is a portal for developeres who use commands frequestly n their day to day life or once in a while usage. We all forget syntax and need quick reference rather than going thru the offical pages.  

  - This repo contains json file for each framework, tool, etc. which requires contribution
  - The repo for allcommands.io portal is [here](https://github.com/shutron/AllCommands.Portal). Feel free to contribute there as well 

# Setup


# How To Contribute
> Its extremely simple to contribute. The follwing 3 steps is all needed to contribute. Each steps are explained with pictures.

If you are already familiar with git go ahead and do it your own way.

### Step 1. Create a branch from `master` branch
+ Go to allcommands [repositary](https://github.com/shutron/AllCommands)  and click on branch
+ Enter any sutiable branch name of your choice and click on create branch
+ Now you can see your newly created branch 

### Step 2. Add in new commands in the existing files / create new file for a new framework, tool and add in commands for that in the newly created branch
+ If you want to add commands for a framework/ tool which doesnt have `.json` file, 
    * Click on `Create new file`
    * Add your framework/ tool name. e.g. `powershell.json`
    * Add in your commands. (Please find here for the file format) 
    * Commit new file
+ If you want to add more commands to an existing file
    * Click on the file (e.g. got.json)
    * Click on edit and add your new commands
    * Commit the changes

### Step 3. Create a `pull request` to master branch
+ Select your branch and click on `New pull request` button
+ add any comments (optional) and click on `Create pull request` button

That's all needed to contribute. One of the reviewer will merge it into the master and the commands will be visible in allcommands.io portal which will be used by many developers.


# JSON format

```json
{
   "category":"powershell",
      "release":{
         "version":"1.0",
         "commands":[
            {
               "command":"Test-Path",
               "description":"Test-Path lets you verify whether items exist in a specified path",
               "usage":"Test-Path <FILE PATH>"
            },
            {
               "command":"Start-Sleep",
               "description":"To suspend the activity in a script or session",
               "usage":"Start-Sleep -Seconds <Seconds>",
               "options":[
                  {
                     "value":"Seconds",
                     "description":"sleep in seconds",
                     "usage":"Start-Sleep -Seconds <Seconds>"
                  },
                  {
                     "value":"Milliseconds ",
                     "description":"sleep in milliseconds",
                     "usage":"Start-Sleep -Milliseconds <Milliseconds>"
                  }
               ]
            }   
       ]
      }
}
```
### JSON format Explained

Key  | Description
------------- | -------------
category  | Content Cell
release  | Content Cell 
version  | Content Cell 
commands  | Content Cell 
command  | Content Cell 
description  | Content Cell 
usage  | Content Cell 
options  | Content Cell 
value  | Content Cell 
usage  | Content Cell 

