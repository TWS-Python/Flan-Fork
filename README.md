
Flan





Overview
Flan is a powerful server-side land claiming mod for Minecraft using the Fabric modding platform. Enhance your multiplayer experience by allowing players to claim and manage their territories with ease!

Features
Intuitive Land Claiming: Players can claim land easily and effectively, ensuring their builds are protected from unwanted interference.
Customizable Permissions: Tailor land management permissions to fit your server’s needs.
Multi-Language Support: Now you can contribute translations! Add your language under common/src/main/resources/data/flan/lang.
Getting Started
To include Flan in your project dependencies, add the following snippet to your build.gradle file:

groovy
Copy code
repositories {
    maven {
        name = "Flemmli97"
        url "https://gitlab.com/api/v4/projects/21830712/packages/maven"
    }
}

dependencies {    
    // Fabric Dependencies
    modCompileOnly("io.github.flemmli97:flan:${minecraft_version}-${flan_version}-${mod_loader}:api") {
        transitive = false // Set to true to include optional dependencies
    }
    modRuntime("io.github.flemmli97:flan:${minecraft_version}-${flan_version}-${mod_loader}") {
        transitive = false // Set to true to include optional dependencies
    }
}
Contributing
We welcome contributions! If you'd like to submit a translation or suggest features, please join our Discord server or create a pull request on our GitHub.

Support
For any issues or support requests, please reach out on our Discord or open an issue on our GitHub repository.

Thank you for choosing Flan! Enjoy building and protecting your worlds in Minecraft!
