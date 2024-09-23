# Flan

[![CurseForge Fabric](http://cf.way2muchnoise.eu/full_404578_Fabric_%20.svg)](https://www.curseforge.com/minecraft/mc-mods/flan)  
[![CurseForge Forge](http://cf.way2muchnoise.eu/full_493246_Forge_%20.svg)](https://www.curseforge.com/minecraft/mc-mods/flan-forge)  
[![Modrinth Downloads](https://img.shields.io/modrinth/dt/Si383TIH?logo=modrinth&label=Modrinth)](https://modrinth.com/mod/flan)  
[![Modrinth Game Versions](https://img.shields.io/modrinth/game-versions/Si383TIH?logo=modrinth&label=Latest%20for)](https://modrinth.com/mod/flan)  
[![Discord](https://img.shields.io/discord/790631506313478155?color=0a48c4&label=discord)](https://discord.gg/8Cx26tfWNs)

## Overview

**Flan** is a server-side land claiming plugin for Minecraft Fabric. This mod allows players to claim land, enhancing the gameplay experience by providing a secure area for building and protecting resources.

### Key Features

- **Land Claiming**: Players can easily claim land to protect their builds from other players.
- **Configurable Settings**: Adjust claim sizes, permissions, and other settings through a simple configuration file.
- **Translation Support**: Easily contribute translations to make the mod accessible to a wider audience.
- **Lightweight**: Designed to minimize server performance impact, making it suitable for both small and large servers.

## Installation

1. **Download the Mod**: Get the latest version of Flan from [CurseForge](https://www.curseforge.com/minecraft/mc-mods/flan) or [Modrinth](https://modrinth.com/mod/flan).
2. **Install Fabric**: Ensure you have the Fabric mod loader installed on your server.
3. **Place the Mod**: Add the downloaded JAR file to your server's `mods` folder.
4. **Restart the Server**: Restart your server to load the mod.

## Contributing Translations

You can contribute translations to the mod. Please place your translation files under:

```
common/src/main/resources/data/flan/lang
```

For example, to add a new language, create a file named `your_language_code.json` in the `lang` folder.

## Configuration

After installing, you can configure Flan by editing the `flan.properties` file located in the `config` folder. Here are some of the settings you can adjust:

- **Claim Size**: Set the maximum size for claims.
- **Claim Duration**: Define how long a claim lasts before needing renewal.
- **Permissions**: Configure permissions for different player roles (admins, members, etc.).

## Adding Flan to Your Project

To use Flan in your dependencies, add the following snippet to your `build.gradle` file:

```groovy
repositories {
    maven {
        name = "Flemmli97"
        url "https://gitlab.com/api/v4/projects/21830712/packages/maven"
    }
}

dependencies {    
    // Fabric
    modCompileOnly("io.github.flemmli97:flan:${minecraft_version}-${flan_version}-${mod_loader}:api") {
        transitive = false // Remove this if you want to include optional dependencies
    }
    modRuntime("io.github.flemmli97:flan:${minecraft_version}-${flan_version}-${mod_loader}") {
        transitive = false // Remove this if you want to include optional dependencies
    }
}
```

## Troubleshooting

If you encounter issues while using Flan, consider the following:

- **Check Compatibility**: Ensure you are using compatible versions of Minecraft, Fabric, and Flan.
- **Review Logs**: Check the server logs for any error messages related to Flan.
- **Community Support**: Reach out on our [Discord](https://discord.gg/8Cx26tfWNs) for help from the community.

## License

Flan is released under the [MIT License](LICENSE).

---

For more information, please visit the [official documentation](https://www.example.com/documentation) or join our [Discord community](https://discord.gg/8Cx26tfWNs)!
