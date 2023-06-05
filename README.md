# arcdps-update-linux

Original PowerShell script found at https://blog.alexdpsg.net/958/

Converted to Shell for usage on Linux.

Edit the file first to make sure the path to Guild Wars 2 folder is correct. (By default: `"$HOME/.local/share/Steam/steamapps/common/Guild Wars 2"`)

Make sure the file is executable (if it's not, use the command below) and place it in a folder from your `$PATH`.
```
chmod +x arcdps-update
``` 

Now you can open a terminal and launch the update with `arcdps-update`. (Will not launch Guild Wars 2 afterward)

If there was a new version downloaded, it will also download the changes from the homepage and display them.

## Example of output
```
Opening /home/mika/.local/share/Steam/steamapps/common/Guild Wars 2
d3d11.dll last modified: Tue 28 Mar 23:29:57 CEST 2023
Downloading md5sum...
Checking md5sum...
ArcDps is out of date
Downloading ArcDps...
Completed ArcDps install
Loading changes...
1,7d0
< may.02.2023: fixed a rare crash that could happen after changing per-agent historical.
< may.02.2023: added option for duration disconnected/off-map squad member history is kept.
< may.02.2023: replaced ugly buff table buff list arranger with drag and drop.
< may.02.2023: use subgroup 1 colour for buff table as default (not 0/grey).
< may.02.2023: added buff table per-buff option to override calculating uptime as intensity or duration (hit/poll only).
< may.02.2023: added keybind options for metrics, self stats, self skills, default unbound.
< may.02.2023: undocumented fixes (or breaking things).
```
