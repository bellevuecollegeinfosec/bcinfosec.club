---
title: "How to Get Access to InfoSec Internal Resources"
---

{{< callout context="note" title="Note" icon="outline/info-circle" >}}
To even begin accessing internal resources you must be added to the **Bellevue College InfoSec SSO list**, if you are not added, you can request to be added by [filling out this form](https://forms.office.com/r/K3keHmA44n) or by attending a meeting in-person.

Unfortunately this process is not automated, as such, please give up to a week (during active quarters).

If the process is taking to long reach out to: `infosec@bellevuecollege.edu`
{{< /callout >}}

# Accessing Internal Webpages

Currently the only accessible webpages to the open internet are:
- Our CTF platform: [ctf.bcinfosec.club](https://ctf.bcinfosec.club)
- Our instance of Juice Shop: [juice.bcinfosec.club](https://juice.bcinfosec.club)

# Accessing Personal Docker Container

To access your personal docker container you must set up an SSH tunnel using `cloudflared`.

## Windows

{{< callout context="note" title="Note" icon="outline/info-circle" >}}

If you do not already have them installed:

### PuTTY - Terminal emulator with lots of functionality including support for `telnet`, `ssh`.

You can get PuTTY from: [https://www.putty.org/](https://www.putty.org/)

**OR**

By running this command in your terminal:

```
winget install -e --id WinSCP.WinSCP
```


### WinSCP - Graphical-User-Interface for SSH/SFTP/FTP file transfer on Windows.

You can get WinSCP from: [https://winscp.net/eng/download.php](https://winscp.net/eng/download.php
)

**OR**

By running this command in your terminal:

```
winget install -e --id WinSCP.WinSCP
```

{{< /callout >}}

Once both `PuTTY` and `WinSCP` have been installed, open `WinSCP`.

In WinSCP upon opening select `💻 New Site`, then select `Advanced...`, from there head to `Connection > Proxy`.

Under `Proxy type:` select `Local`, then under `Proxy settings > Local proxy command:` paste this:

```
cloudflared access ssh --hostname ssh.bcinfosec.club
```

Once entered, confirm your changes by pressing `OK`.

You should land back at the `💻 New Site` page, in the `hostname` field put:

```
ssh.bcinfosec.club
```

In the `username` field put your name formatted like:

```
<firstname>.<lastname>
```

Then put your password in the `password` field.

Finally, press the `🔽` button next to `Login` and select `Open in PuTTY`, or press `Ctrl + P`

## MacOS

Install `cloudflared` using Homebrew:

```shell
brew install cloudflared
```

Add the following to your ssh `config` file at the path: `~/.ssh/config`:

```shell
Host ssh.bcinfosec.club
ProxyCommand /opt/homebrew/bin/cloudflared access ssh --hostname
%h
```

## Linux

Install `cloudflared` using their [package repositories](https://pkg.cloudflare.com/index.html) or [by downloading the cloudflared binary, .deb, .rpm, etc.](https://developers.cloudflare.com/cloudflare-one/connections/connect-networks/downloads/#linux)

Add the following to your ssh `config` file at the path: `~/.ssh/config`:

```shell
Host ssh.bcinfosec.club
ProxyCommand /usr/local/bin/cloudflared access ssh --hostname %h
```

{{< callout context="note" title="Note" icon="outline/info-circle" >}}
If you get the following error: no such file or directory:
`/usr/local/bin/cloudflared` or something similar. Run the command which
cloudflared and replace the path in `~/.ssh/config` with the one it outputs.
{{< /callout >}}

## SSH command (MacOS & Linux)

Finally after updating your ssh config on either:

In your terminal, run `ssh <firstname>.<lastname>@ssh.bcinfosec.club`

{{< details "Example" open >}}

`ssh jack.jackson@ssh.bcinfosec.club`

{{< /details >}}

A browser window should open, hit `accept`.

Back on the terminal, enter your password.

⬆ Elaborate??
