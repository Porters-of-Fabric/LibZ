# LibZ
LibZ is a library for a few mods made by Globox_Z.

## Disclaimer
>[!WARNING]
> This is an updated version of LibZ for 1.21.2 and upwards.\
> **Do not report any bugs to the original developer!**
> All bug reports should go to https://github.com/Porters-of-Fabric/LibZ/issues.

### Installation
LibZ is a library built for the [Fabric Loader](https://fabricmc.net/). It requires [Fabric API](https://www.curseforge.com/minecraft/mc-mods/fabric-api) and [Cloth Config API](https://www.curseforge.com/minecraft/mc-mods/cloth-config) to be installed separately; all other dependencies are installed with the mod.

### License
LibZ is licensed under MIT.

### For Mod Developers
Bring in the library as a dependency:

Register the repository and maven dependency as shown below:
```groovy
repositories {
    maven { url "https://repo.skullian.com/releases" }
}

dependencies {
    modApi ("net.libz:libz:${libz_version}") {
		exclude(group: "net.fabricmc.fabric-api")
	}
}
```

Set the required version for libz in the `gradle.properties`:
```
    libz_version=1.21.2-1.0.5
```

For the required version check out the [versions](https://modrinth.com/mod/libz/versions) tab on Modrinth.