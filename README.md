# Multiplayer fix for AoE 2: DE
To reach the steam launch options you go to Age of Empires Definitive Edition and go to it's properties, there you find launch options.

This script checks if ucrtbase.dll is installed for AoE2: DE then installs it if necessary. To run automatically before launching AoE, set your Steam launch options to

```
location/of/script/run.sh ; %command% %steam_location%
```

for example, if you cloned the repo to your $HOME directory,

```
~/proton_aoe2de_mpfix/run.sh ; %command% %steam_location%
```

if %steam_location% is not set, the script will default to /home/$USER/.steam/steam



## Dependencies or packages needed
Depending on the distribution installing these packages can vary. Google your way through to how to install these packages.
- cabextract
- wget
- jq (optional, required to automatically fetch Steam App ID)
