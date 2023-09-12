
# zitCraft 3

- [zitCraft 3](#zitcraft-3)
  - [Description](#description)
    - [**Key Features**](#key-features)
    - [**Rediscover, Rebuild, and Redeem**](#rediscover-rebuild-and-redeem)
  - [Modpack Homepage](#modpack-homepage)
  - [\[For Developers\] More Info](#for-developers-more-info)
    - [How to create a NEW modpack using PAX](#how-to-create-a-new-modpack-using-pax)
    - [Running the modpack](#running-the-modpack)

## Description

Embark on a journey of redemption in zitCraft 3, a modpack that marks a triumphant return after a hiatus since 2015. This time, the adventure is imbued with the spirit of redemption, offering a fresh perspective on Minecraft's ever-evolving world.

### **Key Features**

-   **A Second Chance:** zitCraft 3 is more than just a modpack; it's a testament to the power of redemption. Rediscover the joy of Minecraft with a meticulously crafted collection of mods that breathe new life into the game.
-   **Themes of Redemption:** From the depths of forgotten dungeons to the soaring heights of rebuilt civilizations, every aspect of zitCraft 3 resonates with the theme of redemption. Unearth lost treasures, restore ancient relics, and witness the transformation of a world once in disarray.
-   **Forging New Paths:** This time, the journey is different. The challenges you faced in 2015 are but echoes of the past. In zitCraft 3, you'll navigate a world that has been redefined, offering fresh trials and triumphs for both new and returning players.
-   **Community-Driven Renaissance:** Your return marks a new chapter in the zitCraft legacy. Share your insights, suggestions, and experiences as we collectively breathe life back into this world of redemption.

### **Rediscover, Rebuild, and Redeem**

zitCraft 3 is an invitation to rekindle your passion for Minecraft, to forge a path of redemption in a world that welcomes you back with open arms. Are you ready to embark on this journey of renewal and rediscovery?

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
- Go here to find you CurseForge API Token: https://legacy.curseforge.com/account/api-tokens

### Running the modpack
ServerStarter: https://github.com/BloodyMods/ServerStarter
