# RI-MSTeams Policy Files
A collection of policy files containing settings for Microsoft Teams accounts in Raffles Institution.\
The files tell you what each account can do in MS Teams. Useful if you wish to check if certain features of MS Teams are not working due to policy set by IT Dept.\
Any potentially identifiable information has been stripped off to protect privacy of accounts which extracted the files.
## How were these files extracted?
When Microsoft Teams starts, a request to https://teams.microsoft.com/api/mt/apac/beta/users/useraggregatesettings will be sent, with a JSON file containing all policies downloaded. The Microsoft Teams app will enable/disable functions based on the settings it received. \
These files for various accounts have been compiled here for ease.
## Are there any sections that are of significant interest?
Yes! I strongly recommend you to check out the "meetingPolicy" section. You can do a CTRL+F or CMD+F to find it when you click on one of the files.
## Can I customise my Microsoft Teams with these files (and enable/disable various features)?
Yes! Download a web inspector and set it to return your edited response (just search how to use one) when https://teams.microsoft.com/api/mt/apac/beta/users/useraggregatesettings is requested. Feel free to download the pre-existing JSON files here and you may optionally customise it in VS Code or any IDE before putting it in your web inspector.
## What about JSON configuration files for teacher/staff accounts?
Hold on, I'm finding one.
## What is this useraggregatesettings (unblock all).json file?
It's a non-RI account file that enables all (or at least most features).\
It has more privileges than RI teacher/staff accounts.
## Why are there two JSON files for students?
IT Admin recently relaxed restrictions for student accounts.\
The old file (before 27 July) contains more restrictions (eg Screen Sharing Disabled).\
The new file (updated 27 July) contains less restrictions (eg Screen sharing only allows single application sharing).
