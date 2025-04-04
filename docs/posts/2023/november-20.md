---
title: Debian Linux migration
date: 2023-11-20
authors:
  - practicalli
categories:
  - practicalli
---

Enjoying Debian Linux and freedom from Snaps


<!-- more -->

## Post install

TODO: see `debian-post-install.md` file on Londo laptop


### NordVPN & Nordpass

NordVPN installs via a script

Nordpass for Linux is only available as a snap, so using the website version.

Requested to Nord support that an AppImage package for Nordpass is provided as it does not need all the mechanism of a snap.

> TODO: investigate if there is a firefox plugin for nordpass that doesnt require a separate install (doesnt seem to be the case unfortunately)


## Adminsitration Account

A root user account is created during initial Debian Linux installation, prompting for the root password.

`su -` is used to change from the normal user login to the root account, allowing for package updates and other Adminsitrative commands to be run.

!!! NOTE ""
    ```shell
    su -
    ```

Enter the root password when prompted.

Carry out administrative tasks as required and type `exit` to leave the root account and return to the user account.


!!! HINT "Dedicated terminal console"
    Use a dedicated terminal session when undertaking many administrative tasks by login in as root once.  Terminal appls like [Kitty](https://practical.li/engineering-playbook/os/command-line/kitty-terminal/){target=_blank}) can open multiple tabs, so one of the tabs can be used to `su -` to the root account.

    [:fontawesome-solid-book-open: Kitty Terminal - Practicalli Engineering Playbook](https://practical.li/engineering-playbook/os/command-line/kitty-terminal/){target=_blank .md-button}

---
Thank you.

[:globe_with_meridians: Practical.li Website](https://practical.li){target=_blank .md-button}

[:fontawesome-brands-github: Practical.li GitHub Org](https://github.com/practicalli){target=_blank .md-button}
[:fontawesome-brands-github: practicalli-johnny profile](https://github.com/practicalli-johnny){target=_blank .md-button}

[:fontawesome-brands-mastodon: @practicalli@clj.social](https://clj.social/@practicalli){target=_blank .md-button}
[:fontawesome-brands-twitter: @practical_li](https://twitter.com/practcial_li){target=_blank .md-button}
