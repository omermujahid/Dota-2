Dota-2
==============

This is the README for the Dota 2 Linux and Mac Beta.

Please use this repository to report bugs for Dota 2 on Linux and Mac.

**PLEASE NOTE: The game is in early Beta and there is a number of known issues; PLEASE make sure to check the issues list and do a search for your symptoms before filing a new one!**

Conduct
-------

There are basic rules of conduct that should be followed at all times by everyone participating in the discussions.  While this is generally a relaxed environment, please remember the following:

- Do not insult, harass, or demean anyone.
- Do not intentionally multi-post an issue.
- Do not use ALL CAPS when creating an issue report.
- Do not repeatedly update an open issue remarking that the issue persists.

Remember: Just because the issue you reported was reported here does not mean that it is an issue with Dota 2.  As well, should your issue not be resolved immediately, it does not mean that a resolution is not being researched or tested.  Patience is always appreciated.

Reporting Issues
----------------

If you encounter a bug while using Source 1 games, first search the [issue list](https://github.com/ValveSoftware/Dota-2/issues) to see if it has already been reported. Include closed issues in your search.

If it has not been reported, create a new issue with at least the following information:

- what platform this is occuring on: Linux or Mac;
- a short, descriptive title;
- a detailed description of the issue, including any output from the command line;
- steps for reproducing the issue; and
- your [system information](#system-information).

Please place logs either in a code block (press `M` in your browser for a GFM cheat sheet) or a [gist](https://gist.github.com).

### System information

Your system information must include:
- your Linux distro or Mac OS version
- if Linux, your Desktop/Window Manager
- if Mac, the model and revision of your hardware
- your Graphics card info (manufacturer, card version), any and all graphics driver versions
- anything else that you think may be useful (mouse/keyboard, filesystem type, etc).

The preferred and easiest way to get this information is from Steam's Hardware Information viewer from the menu (`Help -> System Information`).

Once your information appears: right-click within the dialog, choose `Select All`, right-click again, and then choose `Copy`.
Paste this information into your report, preferably in a code block or a [gist](https://gist.github.com).

Feature Requests
-------------------

This repository is not meant for Dota 2 feature requests. There are forums dedicated to general Dota 2 discussion at http://dev.dota2.com.

Driver Contact Information
--------------------------

Some of the issue you may be experiencing are due to the various video drivers.  Here is an incomplete list of places that you might be able to file bugs or get additional help:

### AMD

AMD Steam Linux forum for reporting **compatibility and performance issues with AMD hardware**:

http://devgurus.amd.com/community/steam-linux

The AMD Open Source driver is a part of Mesa, so use the links under "Intel" to report issues with it.

### Intel

For discussions, there is the mesa-users email list:

http://mesa3d.org/lists.html

Bugs and feature requests should be logged in bugzilla:

http://mesa3d.org/bugs.html

### NVIDIA

NVIDIA supported drivers
- https://devtalk.nvidia.com/default/board/98

Open Source NVIDIA driver (nouveau)
- http://nouveau.freedesktop.org/wiki/FrontPage

If you know of any other places, please let us know.

Known Video Driver/Card issues:
----------------------------------

### NVIDIA

6xxx and 7xxx hardware have been EOL'd. The code specific to these GPUs isn't even compiled into drivers anymore.

6xxx and 7xxx GPUs are incapable of performing sRGB functionality needed by Source Engine titles when being driven by OpenGL. (The sRGB behavior as specified in OpenGL is slightly different than the behavior that was actually unspecified in D3D9, which is why this works in D3D9 but not in OpenGL).

