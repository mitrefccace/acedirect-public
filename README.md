# ACE Direct

![AD](images/adsmall.png)

Accessible Communications for Everyone (ACE) Direct is a Direct Video Calling (DVC) platform that enables direct calling from deaf and hard-of-hearing individuals to an American Sign Language (ASL)-trained agent within an organization's call center. The agent handles the call using a video-capable phone with real-time video connection. To demonstrate the capabilities of DVC, the FCC and CAMH have further advanced the original auto-routing POC into a call center platform for two to ten customer service representatives.

## Release v4.0

The latest release of ACE Direct is **Release v4.0**. See the [RELEASENOTES.md](RELEASENOTES.md) file for the changes included in this release.

## Clean Installation

To install ACE Direct from scratch, see the [CHECKLISTS.md](CHECKLISTS.md) file. This file describes the installation and configuration process for the ACE Direct system.

## Getting the Latest Software

If you only want to download the latest software, start here. The latest release includes several Git **submodules** in this repo. Please pull the Git submodules linked here, for example:

```sh
$  git clone git@github.com:mitrefccace/acedirect-public.git  # get top repo
$
$  cd acedirect-public
$  git fetch origin v4.0
$  git checkout v4.0
$  git submodule init  # initialize local config file
$  git submodule update --init --remote --recursive  # get individual repos
```

Next, go to *each* individual repo and get the correct version. For example, for the `acedirect` repo::

```sh
$  cd acedirect
$
$  git fetch origin v4.0
$  git checkout v4.0
$  git pull origin v4.0
```

Repeat for all other individual repos. _Note that some repos only have a **master** branch, since they are compatible with all versions of ACE Direct_.

## Documentation

Please see the *docs* folder for official documentation on the project overview, installation, and configuration. See the README.md files in the Git submodules for installation and configuration details of those individual repos.
