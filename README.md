![GRID0+ emu](img/banner.png)

# GRID0+ emu
[![Chat on Discord](https://img.shields.io/badge/Discord-5865f2?logo=discord&logoColor=white)](https://discordapp.com/invite/splatfest)

**Play Switch games online with friends over custom servers (GRID0+) OR a virtual LAN (GRID0).<br>
Emulator builds for Ryujinx and Citron (including Citrosis).**

<sub>**GRID0+:** Replaces NSO functionality for online matchmaking, Splatfests, and in-game progression.</sub><br>
<sub>Works for cross-play with banned switch users. Runs on custom servers. More info at [GRID0+](https://github.com/GRID0-net/GRID0).</sub><br>
<sub>**GRID0:** Replaces the old LAN-play relays with better stability, faster speeds, and an easier setup.</sub><br>
<sub>Works for cross-play with unbanned and banned switch users. Runs on ZeroTier. More info at [GRID0](https://github.com/GRID0-net/GRID0).</sub>

#### Which emulator should I use?

<details>
<summary><b>Flowchart</b></summary>

```mermaid
graph TD
    A[Do you have a Mac?] --> B{Yes}
    A --> C{No}
    B --> D{Intel or Silicon?}
    D -->|Intel| E[Ryujinx]
    D -->|Silicon| F[Citrosis<br/>native Swift UI, Metal renderer]
    C --> G{Is your CPU from 2019 or newer?}
    G -->|Yes| E
    G -->|No| I[Citron<br/>better on weak hardware]
    click E "https://github.com/GRID0-net/GRID0-ryu"
    click I "https://github.com/GRID0-net/GRID0-citron"
```

</details>

<details>
<summary><b>If the flowchart above doesn't render, use this:</b></summary>
<p align="center">Are you using a Mac?<br><sub>(An Apple computer)</sub></p>
<div align="center">
<table>
<tr>
<td valign="top">
<details>
<summary><b>Yes</b></summary>
<p align="center"><b>Intel or Silicon?</b><br><sub><a href="https://support.apple.com/en-us/HT211814">Check if your Mac has Apple Silicon or Intel</a></sub></p>
<div align="center">
<table>
<tr>
<td valign="top">
<details>
<summary><b>Intel</b></summary>

<p align="center">Considering you are on an Intel Mac, the best emulator for you is<br><a href="https://github.com/GRID0-net/GRID0-ryu"><b>Ryujinx</b></a></p>

</details>
</td>
<td valign="top">
<details>
<summary><b>Silicon</b></summary>

<p align="center">Considering you are on a Silicon Mac, the best emulator for you is<br><a href="https://github.com/GRID0-net/GRID0-citron/releases"><b>Citrosis</b></a> <i>(native Swift UI, Metal renderer)</i></p>

</details>
</td>
</tr>
</table>
</div>
</details>
</td>
<td valign="top">
<details>
<summary><b>No</b></summary>
<p align="center"><b>How old is your CPU?</b><br><sub><a href="https://en.wikipedia.org/wiki/List_of_Intel_processors">Look up your Intel CPU release date</a> · <a href="https://en.wikipedia.org/wiki/Table_of_AMD_processors">Look up your AMD CPU release date</a></sub></p>
<div align="center">
<table>
<tr>
<td valign="top">
<details>
<summary><b>From 2019 or newer</b></summary>

<p align="center">Considering you are on a relatively new non-Mac, the best emulator for you is<br><a href="https://github.com/GRID0-net/GRID0-ryu"><b>Ryujinx</b></a></p>

</details>
</td>
<td valign="top">
<details>
<summary><b>Older than 2019</b></summary>

<p align="center">Considering you are on a relatively older non-Mac, the best emulator for you is<br><a href="https://github.com/GRID0-net/GRID0-citron"><b>Citron</b></a></p>

</details>
</td>
</tr>
</table>
</div>
</details>
</td>
</tr>
</table>
</div>
</details>
<hr>


## Setup Guide

Runs directly on the console as a background sysmodule. No PC or phone required while playing.

1. Download the latest release from the **[GRID0+ cfw](https://github.com/GRID0-net/GRID0plus-cfw/)** repository.
2. Extract the archive to the root of your SD card.

[image: the SD card root with the extracted sys-GRID0 folders in place]

**GRID0:**
3. Reboot into Atmosphere, (temporary step) Currently the network id isnt included with the release, so in ultrahand, insert the following network id on the sys-zerotier page (name is also not yet updated) : 8bd5124fd68185ec
4. Verify connection status using the Tesla (or Ultrahand) overlay menu.

[image: the Tesla overlay open on the Switch showing the sys-GRID0 connection status]

**GRID0+:**
3. Reboot into Atmosphere, open the HomeBrew Menu (Album), open the GRID0+ Toolbox and select Change to GRID0+ mode.
4. After your switch restarts, head to Settings > Users > Add A User > Not With Me > Yes, Had an Account > Link Account > Sign Into Your GRID0+ account using your Discord username and password from the bot.
5. Verify connection status using the Tesla (or Ultrahand) overlay menu.

[image: the Tesla overlay open on the Switch showing the sys-GRID0 connection status]

---

<sub>Built by 3 humans with limited AI assistance, tested on real Switches over many days and restless nights.
