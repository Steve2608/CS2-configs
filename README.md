# Setup

- create a symlink to the cfg folder of cs2:
```ps1
$config_dir=pwd
$cs2_dir="S:\SteamLibrary\steamapps\common\Counter-Strike Global Offensive\game\csgo\cfg"

cd $cs2_dir
New-Item -Path startup.cfg -ItemType SymbolicLink -Value "${config_dir}\startup.cfg"
New-Item -Path nade_practice.cfg -ItemType SymbolicLink -Value "${config_dir}\nade_practice.cfg"
```

- add `+exec startup.cfg` to your cs2 launch options
