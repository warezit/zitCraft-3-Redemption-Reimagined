# zitCraft 3

- [zitCraft 3](#zitcraft-3)
  - [Description](#description)
  - [Modpack Homepage](#modpack-homepage)
  - [\[For Developers\] More Info](#for-developers-more-info)
    - [How to create a NEW modpack using PAX](#how-to-create-a-new-modpack-using-pax)
    - [\[For Developers\] Running the](#for-developers-running-the)

## Description
Updates coming soon!

## Modpack Homepage
zitCraft 3: https://legacy.curseforge.com/minecraft/modpacks/zitcraft-3

## [For Developers] More Info

This project uses PAX to manage the modpack: https://github.com/froehlichA/pax
- Download PAX, then extract to the root folder of the repo.
- PAX *must* be run from the root folder of the repo.

### How to create a NEW modpack using PAX

These steps show I created this modpack, so I can refer back to these steps later if needed. These steps may work for you, or may not. YMMV.

- Make a new folder
- Download PAX, then extract the .ZIP to the folder you just created
- Run `.\pax.exe init` to initialize the modpack file structure
- For Fabric modpacks, run this to install the FabricAPI mod (required for any Fabric modpacks) `.\pax.exe add https://www.curseforge.com/minecraft/mc-mods/fabric-api`
- List the current mods by running `.\pax.exe list`
- Export the modpack by running `.\pax.exe export`. This will generate a new folder named `.old` (required for using Automatic Deployment later), then export a .zip file of the modpack.
- Generate the appropriate GitHub action file for your project by running this command `.\pax init -f skip-manifest`. More info [here](https://github.com/froehlichA/pax/issues/26#issuecomment-864464285).
- Then [follow the rest of the Continuous Deployment setup here](https://github.com/froehlichA/pax/wiki/Automatic-releases). (Get an API Key and the CurseForge Project ID, then modify the GitHub action file we just created.)

### [For Developers] Running the 
ServerStarter: https://github.com/BloodyMods/ServerStarter
