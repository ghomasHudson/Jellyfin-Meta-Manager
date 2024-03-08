This is a Work-In-Progress conversion of [Plex Meta Manager](https://github.com/meisnate12/Plex-Meta-Manager) to use the Jellyfin API.


### First steps
Have considered porting python-plexapi to create a jellyfin equivilent [python-jellyfinapi](https://github.com/ghomasHudson/python-jellyfinapi). Basic things like logging in is quite easy but filtering gets a bit complex (the APIs are quite different).


For now try using [Jellyfin Auto Collections](https://github.com/ghomasHudson/Jellyfin-Auto-Collections).

----------------
## WIP

Jellyfin Meta Manager is a powerful tool designed to give you complete control over your media libraries. With Jellyfin Meta Manager, you can take your customization to the next level, with granular control over metadata, collections, overlays, and much more.

Transform your media library with Jellyfin Meta Manager and discover its full potential! Connect to third-party services like TMDb, Trakt, and IMDb, among others, to create one-of-a-kind collections, overlays and more. Your media library will stand out and be tailored to your specific needs.

## What Can Jellyfin-Meta-Manager Do?

### Overhaul Your Media Libraries

-  Elevate your library with beautifully crafted metadata - customize artwork, titles, summaries, and more to create a stunning library.

### PMM Defaults

-  Take advantage of pre-made modular Collections & Overlays to reduce the manual effort and get to the good stuff with less effort!

### Third-Party Integrations

-  Harness the power of Trakt, TMDb, IMDb, Flixpatrol and more to create collections and overlays!
-  Integrate with Sonarr and Radarr to automate your library growth.

### And More!

-  We're constantly working on new features to take your library management experience to the next level.
-  Consider sponsoring the project to allow us to continue building great features for you!

## Example Jellyfin Meta Manager Libraries 

Here are some examples of the things you can achieve using Jellyfin Meta Manager!

**Example Movie Collections using the [Jellyfin Meta Manager Defaults](https://metamanager.wiki/en/latest/defaults/collections/)** (click to enlarge):

![Movie Collection Preview](https://metamanager.wiki/en/latest/images/movie-collection-preview.png)

**Example Show Overlays using the [Jellyfin Meta Manager Defaults](https://metamanager.wiki/en/latest/defaults/collections/overlays)** (click to enlarge):

![Show Library Preview](https://metamanager.wiki/en/latest/images/show-library-preview.png)

## Jellyfin Meta Manager Defaults

Want your library to look like the above images?  With the [PMM Defaults](https://metamanager.wiki/en/latest/defaults/guide/) you can! These powerful and modular files were designed by the Jellyfin Meta Manager team to make it simple to create a personalized, one-of-a-kind media collection without the hassle of manually defining each one.

Want to see what the community has to offer? Check out the [Jellyfin Meta Manager Configs](https://github.com/ghomasHudson/Jellyfin-Meta-Manager-Configs) repository on GitHub to see user-submitted configuration files, or even add your own to the mix!

With Jellyfin Meta Manager, you can also manage metadata for all your media types, from movies and shows to music and more. And since your metadata is managed outside your libraries, you'll never have to worry about losing your customizations in the event of a media server database loss, you can simply reapply them! It is also easy to move your customizations between servers if you need to.

## Getting Started

To get started with Jellyfin Meta Manager, follow these simple steps:

1. Install Jellyfin Meta Manager on your device. You can find the installation instructions for a variety of platforms [here](https://metamanager.wiki/en/latest/pmm/install/overview/).

2. Once you have installed Jellyfin Meta Manager, create your [Configuration File](https://metamanager.wiki/en/latest/config/overview/). This file contains important information such as URLs and credentials needed to connect to services like Jellyfin and TMDb

3. After creating the Configuration File, you can start updating Metadata and building automatic Collections by creating a [Collection File](https://metamanager.wiki/en/latest/files/collections/) for each Library you want to work with. If you'd rather use some of our pre-made Collection Files, take a look at the [Jellyfin Meta Manager Defaults](https://metamanager.wiki/en/latest/defaults/guide/)

4. Finally, check out the [Wiki](https://metamanager.wiki/), you'll find new and exciting ways to truly unlock the potential of your libraries.

## Step-by-Step Guides

If you're a beginner to the concepts of Python, Git and/or Jellyfin Meta Manager and find the above steps challenging, don't worry. We've got some step-by-step guides that can help you get started. These guides will take you through the process of installing Jellyfin Meta Manager, creating your Configuration File and getting some basic Collections up and running.

For those who need full installation walkthroughs, please refer to the following walkthrough guides:

  * [Local Walkthrough](https://metamanager.wiki/en/latest/pmm/install/local/) - follow this if you are running the script directly on Windows, OS X, or Linux
  * [Docker Walkthrough](https://metamanager.wiki/en/latest/pmm/install/docker/) - this discusses using Docker at the command line

If you are using unRAID, Kubernetes, QNAP, or Synology refer to the following basic guide to Docker container setup for each system:

**this doesn't cover the PMM setup specifics found in the guides above with regard to creating the config file and collection file, so you may want to go through the [Docker Walkthrough](https://metamanager.wiki/en/latest/pmm/install/docker/) first on your computer to gain that understanding.**

  * [unRAID Walkthrough](https://metamanager.wiki/en/latest/pmm/install/unraid/)
  * [Kubernetes Walkthrough](https://metamanager.wiki/en/latest/pmm/install/kubernetes/)
  * [QNAP Walkthrough](https://metamanager.wiki/en/latest/pmm/install/qnap/)
  * [Synology Walkthrough](https://metamanager.wiki/en/latest/pmm/install/synology/)

## Example Usage

Jellyfin Meta Manager puts you in control of your media library by letting you create custom Collections that make discovering and organizing your content a breeze. With powerful search and filtering options, you can build Collections based on popular builders like TMDb, IMDb, Trakt, and many more.

Imagine having Collections like these at your fingertips:

  * Trending and Popular (based on TMDb, IMDb, Trakt, etc.)
  * Streaming Services (like Netflix, Disney+, and more)
  * Networks
  * Studios
  * Genres
  * Actors
  * Decades

Jellyfin Meta Manager gives you endless possibilities to curate and organize your media library any way you want. Create custom Collections and Overlays that fit your unique preferences and make discovering your content effortless.

But if you don't want to spend time manually creating Collections and Overlays, we've got you covered. Check out the [PMM Defaults](https://metamanager.wiki/en/latest/defaults/guide/) - a handcrafted selection of tried-and-tested Collections and Overlays made by the Jellyfin Meta Manager team.

## Develop & Nightly Branches

The Develop and Nightly branches are "beta" versions of Jellyfin Meta Manager that are updated more frequently than the stable version (Master branch). These branches are where bug fixes, new features, and other changes are added before being released to the Master branch.

However, these branches (especially Nightly) are recommended for more technical users who don't mind updating frequently to get the latest changes. Keep in mind that these beta branches may have bugs or other issues that could cause problems with Jellyfin Meta Manager or your media server. So, if you're not comfortable with technical issues, it's best to stick with the Master branch.

<details class="details-tabs">
  <summary>Develop Branch (click to expand)</summary>

[![Develop GitHub commits since latest stable release (by SemVer)](https://img.shields.io/github/commits-since/ghomasHudson/Jellyfin-meta-manager/latest/develop?label=Commits%20in%20Develop&style=plastic)](https://github.com/ghomasHudson/Jellyfin-Meta-Manager/tree/develop)

The [develop](https://github.com/ghomasHudson/Jellyfin-Meta-Manager/tree/develop) branch has the most updated **documented** fixes and enhancements to Jellyfin Meta Manager.  This version is tested and documented to some degree, but it is still an active Develop branch, so there may be rough edges.

Switching to `develop`:
````{tab} Running in Docker
Add ":develop" to the image name in your run command or configuration:
```
ghomasHudson/Jellyfin-meta-manager:develop
```
````
````{tab} Running on the Host
In the directory where you cloned PMM:
```bash
git checkout develop
```
To switch back:
```bash
git checkout master
```
````

If switching to the develop branch, it is recommended to also use the [develop branch of the wiki](https://metamanager.wiki/en/develop/), which documents any changes made from the Master branch.

</details>

<br>

<details class="details-tabs">
  <summary>Nightly Branch  (click to expand)</summary>

[![Nightly GitHub commits since latest stable release (by SemVer)](https://img.shields.io/github/commits-since/ghomasHudson/Jellyfin-meta-manager/latest/nightly?label=Commits%20in%20Nightly&style=plastic)](https://github.com/ghomasHudson/Jellyfin-Meta-Manager/tree/nightly)

**This branch will have squashed commits which can cause `git pull`/`git fetch` to error you can use `git reset origin/nightly --hard` to fix the branch.**

There is also a [nightly](https://github.com/ghomasHudson/Jellyfin-Meta-Manager/tree/nightly) branch which will have the absolute latest version of the script, but it could easily break, there is no guarantee that it even works, and any new features will not be documented until they have progressed enough to reach the develop branch.

Switching to `nightly`:

````{tab} Running in Docker
Add ":nightly" to the image name in your run command or configuration:
```
ghomasHudson/Jellyfin-meta-manager:nightly
```
````
````{tab} Running on the Host
In the directory where you cloned PMM:
```bash
git checkout nightly
```
To switch back:
```bash
git checkout master
```
````

As this branch is subject to extreme change, there is no promise of the feature being documented in the nightly branch of the wiki and all discussions relating to changes made in the nightly branch will be held within the [Jellyfin Meta Manager Discord Server]([https://metamanager.wiki/en/latest/discord/](https://discord.gg/AjTsTcjP)).
</details>


## Discord Support Server

If you're looking for support for any questions or issues you might have, or if you just want to be a part of our growing community, Join the [Jellyfin Meta Manager Discord Server]([https://metamanager.wiki/en/latest/discord/](https://discord.gg/AjTsTcjP)).

## Contributing

If it's a Jellyfin-specific change, by all means add it here. For now we're going to follow the upstream, [Plex-Meta-Manager](https://github.com/meisnate12/Plex-Meta-Manager) so request more general features there. Pull Requests are greatly encouraged.

<br>
