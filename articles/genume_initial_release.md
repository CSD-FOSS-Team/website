# Genume Initial Release

### About

Genume, a **g**raphical **enume**ration tool, provides a graphical user interface to accompany a collection of various enumeration scripts.
Developed by our team, it fully complies with the Free and Open Source tenets, as all the source code is available on [GitHub][github-link].
All code is licensed under GPLv2 to better protect the user's rights.

### Overview

![](absolute-path-to-image/genume-logo.png?raw=true) TODO: complete this.

When launching the GUI utility by either `python3 -m genume` or `make`, the user is greeted with the following window:
![](absolute-path-to-image/greeting_page.png?raw=true) TODO: complete this.
The most noticable structure component is directly below the genume logo; a stack containing several tabs. On start-up, the `about` tab is automatically selected.

Here is a listing of all the tabs and their functionalities, in short:

| Name         | Description                                                               |
| ----         | -----------                                                               |
| about        | Contains author team's credits                                            |
| cpu          | Contains information about the machine's CPU                              |
| disks        | Contains information about the machine's disks, cdrom port and partitions |
| distribution | Contains information about the machine's Linux kernel and distribution    |
| gpu          | Contains information about the machine's GPU                              |
| memory       | Contains information about the machine's available memory                 |
| network      | Contains information about the machine's network drivers                  |
| power        | Contains information about the machine's power source                     |
| software     | Contains version numbers of widely-known Linux apps installed             |
| windows      | Contains information about the machine's WM                               |

It is evident that both hardware and software information is readily accessible to the user, thus enabling genume a useful and powerful utility tool.

Furthermore, there are two more key-components of our software:
 1. A refresh button which renders the user capable of accessing real-time information about the machine while changing its configuration on-the-fly.
 2. The ability to export said information in HTML, JSON, JSON-min & plaintext formats.

Let's have a look at what exactly genume comprises and how it is built.

### Structure

For an interactive structure breakdown, the reader is encouraged to simultaneously be browsing the GitHub [repository][github-repo].

The repository consists of three major sub-directories:
 - `bash_helpers`
 - `genume`
 - `scripts`

Here is a brief mention of what each encapsulate:

| Name         | Description                                                                  |
| ----         | -----------                                                                  |
| bash_helpers | Commands everyone can use to easily contribute by writing additional scripts |
| genume       | The exporters, loggers, registry and GUI code                                |
| scripts      | All bash enumeration scripts genume executes on start-up                     |

The structure of each sub-directory is as follows:
 1. `bash_helpers`
    - ease-of-access custom-made commands
    - information, guidelines and examples on how to use the bash helpers available
 2. `genume`
    - constants such as packaging-related app information, links to assets
    - utilities used in codebase
    - files needed in installation
    - various exporters
    - logging (mostly for debugging issues and transparency)
    - registry handling scripts, running threads, executing children, etc.
    - GUI codebase (e.g. event handlers)
 4. `scripts`
    - guidelines on contributing by writing bash scripts
    - the bash scripts used by genume themselves

### Availability

Genume is designed to be distribution-agnostic and is successfully tested on Ubuntu, Arch, Fedora, even NixOS and RaspberryPi.
The reader is encouraged to try genume on his/hers own distribution and supply the team with relevant feedback.
There are detailed instructions on how to make genume run successfully for Ubuntu/Debian/Raspbian, Fedora and Arch Linux distributions.

### Specifics

Should this section exist?

### More

I'll add stuff here when the question above is answered.

_author_: Orestis Ousoultzoglou TODO: add link.

[github-link]: https://github.com/CSD-FOSS-Team/genume
[github-repo]: https://github.com/CSD-FOSS-Team/genume
