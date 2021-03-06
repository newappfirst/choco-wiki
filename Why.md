## Why Chocolatey?
### What is the purpose of Chocolatey?

How many times do you hear about an awesome tool/application from your friends and want to try it out? How much effort do you go through to set a tool and all of it's requirements up on your machine? Do you realize that all of this manual effort is a pain? It's a pain we are used to! It's something we just do and don't realize we are wasting time doing all of this manual process. And worse, when we install applications it's always... Next Next Next Finish.

There is a better way! Once you start to use Chocolatey to silently install applications, tools, and to quickly set up things on your machine, you will start to realize that it is more of a global automation tool. That makes it an enabler, enabling you to do just about anything. And to repeat it anywhere in the world with little more than an internet connection.

Because Chocolatey is built on top of the NuGet infrastructure, that means you can install packages from Chocolatey.org, NuGet.org, MyGet.org, file shares, directories, custom feeds and from private feeds. That means you can set up your own server (even private) and your own internal packages with more company specific packages.

[[Tell me a story|ChocolateyStory]]

### What is Chocolatey?

Chocolatey helps good developers and system administrators become outstanding developers/sysadmins. Chocolatey goes to *eleven*.

Chocolatey is something **you need if you've ever installed, upgraded, or removed software on Windows**. It is an **existing, proven**, project that was started [over 4 years ago](https://github.com/ferventcoder/nugetpackages/commit/d16ed7ac675395b3bb8ecee90fb13efb03d4b619). For those familiar with \*nix package managers, it is a binary package manager, sort of like yum or apt-get, but for Windows. The words "binary package manager" can be confusing for those who don't know what that means, but bear with me for a few minutes. Chocolatey is a tool that automates all the mundane getting and installing software work for you. You just select what you want installed and within a few minutes, Chocolatey has downloaded and installed (or upgraded) that software without need for further input from you. So **while Chocolatey does the hard work, you can go get some coffee**. Or **sleep**. Or do other more important things.

This may not seem very powerful at first, but imagine when you want to **upgrade all** of the software on your system to the latest, most secure versions, how do you do that now? Right. ***Manually***:

1. Search for most recent version
1. Pick (hopefully) the right download
1. Wait for it to download
1. Unblock it
1. Install it manually (next, next, next anyone?)
1. Hope it didn't install any malware
1. Now do it again for ***EVERY*** piece of software on your system.

![chrisfarley-disbelief](https://cloud.githubusercontent.com/assets/63502/6924749/4e4e23d2-d7a0-11e4-9f4e-a44a02b227f6.gif)

Now contrast that with how you do the same with **Chocolatey**:

1. Open command line.
1. Type `choco upgrade all -y`
1. Walk away

![shia-labeouf-magic-gif](https://cloud.githubusercontent.com/assets/63502/6924713/14521f12-d7a0-11e4-819d-88c46e1a7bfa.gif)
### Why not use an existing Windows package manager?
Believe me, I wanted there to be something existing on Windows that would fit the bill. Package management is not a glorious job. Especially on Windows. It's taking all of the different native installers, archives, and straight executable downloads and making a simple interface for consumers to issue the same install command for all of them. Here are/were my needs:

* Good CLI that is simple to use.
* Main repository that takes packages contributions from the community (and is being maintained).
* Ability to use additional/multiple sources.
* Meta packages that can chain dependencies.
* Virtual packages.
* Packages should be easy to create / maintain.
* Packages should be concise and be able to be created without worrying about distribution rights.
* Unattended installs
* Installation of multiple packages with one command.

To date, Chocolatey does all of this (virtual packages is coming).