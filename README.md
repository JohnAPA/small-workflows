# Small Workflows [![Workflows](https://img.shields.io/badge/More%20Workflows-🎩-purple.svg)](https://github.com/learn-anything/alfred-workflows#readme) [![Thanks](https://img.shields.io/badge/Say%20Thanks-💗-ff69b4.svg)](https://www.patreon.com/nikitavoloboev)
> Small [Alfred](https://www.alfredapp.com/) workflows I use that don't warrant a GitHub repository of their own

##### Contents
- [My Workflows](#my-workflows)
- [Workflow Augmentations](#workflow-augmentations)
- [Personal workflows](#personal-workflows)
- [Contributing](#contributing)

## My Workflows
- [Search websites](search-websites#readme) - Searches on popular websites. I use [Web Searches](https://github.com/nikitavoloboev/alfred-web-searches) and [Searchio](https://github.com/deanishe/alfred-searchio) for all other searches.
- [Search Files](search-files#readme) - A lot of [file filters](https://www.alfredapp.com/help/workflows/inputs/file-filter/) to find files quickly
- [Search Selection](search-selection#readme) - Search selected text on various websites with hotkeys.
- [Search for Content](search-for-content#readme) - Actions to search through the insides of PDF and MindNode documents as well as Contacts.
- [WiFi Tools](wifi-tools#readme) - Check WiFi connection / Restart WiFi / Toggle it on/off.
- [Keyboard control](keyboard-control#readme) - Turn your keyboard on and off.
- [Go play](go-play#readme) - Create [Go Playground](https://play.golang.org) from selected Go code for sharing.
- [Focus](focus#readme) - Start [Focus](https://heyfocus.com) blocking for some time that you specify.
- [Dictionary](dictionary#readme) - Search through dictionary.
- [Useful utilities](useful-utilities#readme) - Only has one utility, to search selected text in Alfred.
- [Month numbers](month-numbers#readme) - Search for a month and copy the month number to your clipboard.
- [Clean Folders](clean-folders#readme) - Trash items from Desktop and clean certain folders like removing .alfredworkflows from ~/Downloads.
- [Folder Search](folder-search#readme) - Search folders from Alfred and open them in Finder/iTerm/Editor.
- [File Actions](file-actions#readme) - Various file actions I made to operate on files and folders.
- [Go to Subreddit](goto-subreddit#readme) - Go to a subreddit that you specify. For searching subreddits, use [this](https://github.com/deanishe/alfred-reddit).
- [Dash Profile Switcher](dash-profile-switch#readme) - Search through your custom [Dash](https://kapeli.com/dash) profiles.
- [Local host](local-host#readme) - Open port that you specify at local host.
- [Objects library](objects-library#readme) - Useful premade objects for workflows.
- [Open with app](open-with-app#readme) - File actions to quickly open file/folder in the application without going to `Open with...` menu.
- [TODO Task](todo-task#readme) - Write a task and display it in middle of screen.
- [Birthday](birthday#readme) - See time passed since your birthday.
- [Dropbox Upload](dropbox-upload#readme) - Upload and share files with Dropbox.

## Workflow Augmentations
Below are workflows that were not made by me, I just augmented them in my own way to make them 'better' (for me).

I often propose these changes to the workflow author so that the change is merged but sometimes the author does not want to accept the change so I am left with my own fork until then. Credit goes to the authors of these awesome workflows

Take a look at the original workflows first, it will most probably work for you well.

- [GitHub Jump](https://github.com/lox/alfred-github-jump) - Quickly jump to GitHub repositories you made/starred. ([My modification](https://github.com/nikitavoloboev/small-workflows/blob/master/augmentations/GitHub%20jump.alfredworkflow?raw=true))
  - I added many modifiers to do different things such as go directly to issues of the workflow, pull requests of it or even clone the repo to a specified directory.
  - I use this workflow many many times a day and it saved me a lot of time. [My modification](https://github.com/nikitavoloboev/small-workflows/blob/master/augmentations/GitHub%20jump.alfredworkflow?raw=true) has over [4,600 repos I starred](https://github.com/nikitavoloboev?tab=stars) that are within 1 second access from you if you want to use that.
- [Dash Search with custom hotkeys](https://github.com/Kapeli/Dash-Alfred-Workflow) - Search Dash docs. ([My modification](https://github.com/nikitavoloboev/small-workflows/blob/master/augmentations/Dash.alfredworkflow?raw=true))
  - I extended it with many custom hotkeys to super quickly search a specific docset in [Dash](https://kapeli.com/dash).
- [Alfred Workflow Directory](https://github.com/jeeftor/AlfredWorkflowDirectory) - Quickly open any Alfred Workflow directory in your Terminal, Finder. ([My modification](https://github.com/nikitavoloboev/small-workflows/blob/master/augmentations/Workflow%20directory.alfredworkflow?raw=true))
  - I changed it so that by default it will cd to the workflow in my current iTerm tab but also it can export workflow to `~/Desktop` (you can change location) or it will open the workflow with an editor (VS Code or Sublime in my case).
- [Directory watches](https://github.com/vitorgalvao/alfred-workflows/tree/master/RecentDownloads) - Search insides of directories and action on things. ([My modification](https://github.com/nikitavoloboev/small-workflows/blob/master/augmentations/Directory%20watches.alfredworkflow?raw=true))
  - I modified a script he once shared to quickly see insides of various directories and action on items of them to do various things opening the path in iTerm or moving the file somewhere.
- [Similar image search](https://github.com/deanishe/alfred-similar-image-search) - Google Image searches based on local files. ([My modification](https://github.com/nikitavoloboev/small-workflows/blob/master/augmentations/Google%20similar%20images.alfredworkflow?raw=true))
  - I modified it so you can take a screenshot and immediately search that screenshot on Google
- [Recent Downloads](https://github.com/ddjfreedom/recent-downloads-alfred-v2) - View `~/Downloads` folder from Alfred and action on contents of it. ([My modification](https://github.com/nikitavoloboev/small-workflows/blob/master/augmentations/Recent%20Downloads.alfredworkflow?raw=true))
	- I modified it by adding few actions like opening the path in iTerm. Or opening the file/folder in VS Code.
- [EggTimer](https://www.alfredforum.com/topic/275-eggtimer-v2-updated-to-20-final/) - Start/Stop/View timers. ([My modification](https://github.com/nikitavoloboev/small-workflows/blob/master/augmentations/EggTimer.alfredworkflow?raw=true))
	- I modified it by making it easy to overwrite one active task. I create timers for some time by passing in `new <mins> Reminder` to `timer` external trigger where `<mins>` stands for minutes. So `new 20 Reminder` will create a running timer for 20 minutes. If I pass in `new 30 Reminder` during these 20 minutes running, it will overwrite the timer and make the 30 min timer countdown instead.
	- I use this as a way to set quick estimates for tasks I am working on so I [focus on working on the task I need](https://wiki.nikitavoloboev.xyz/focusing/focusing.html) for that time and then take a break or change my tasks.

## Personal workflows
Below is a list of workflows that were made for my own personal use and will most certainly not work on your systems unless you change many things in the workflow.

You can take some inspiration or ideas from these workflows if you wish.
- [Manage wiki](https://github.com/nikitavoloboev/small-workflows/blob/master/personal/Manage%20wiki.alfredworkflow?raw=true) - I use it to manage editing and extending my [knowledge wiki](https://github.com/nikitavoloboev/knowledge).

## Contributing
See [contribution guidelines](CONTRIBUTING.md#readme).

## Thank you 💜
You can support me on [Patreon](https://www.patreon.com/nikitavoloboev) or look into [other projects](https://nikitavoloboev.xyz/projects) I shared.

## License
MIT © [Nikita Voloboev](https://www.nikitavoloboev.xyz)
