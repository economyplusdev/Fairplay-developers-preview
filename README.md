# Fairplay Plugin Management

This README provides an overview of how to manage plugins within the Fairplay platform, including plugin customization, user views, and deployments.

## General Plugin Menu
![General Plugin Menu](https://cdn.economyplus.solutions/8lltfdwv.png)  
In the General Plugin Menu, you can view all the plugins owned by the developer organization you are logged into. This interface provides a centralized view, allowing you to manage all plugins with ease.

---

## Plugin-Specific Menu
![Plugin Specific Menu](https://cdn.economyplus.solutions/lsks72td.png)  
In the Plugin-Specific Menu, you can manage individual plugin details, including:

- **Description:** Edit the description that users will see.
- **Advertisement:** Modify any promotional content related to your plugin.
- **Banners:** Update the visual banners that represent your plugin.

This section is where you handle plugin customization and keep all relevant details up-to-date.

## Plugin User View
![Plugin User View](https://cdn.economyplus.solutions/2ubiy2os.png)  
This is what the plugin looks like to general users browsing or installing your plugin. Ensure that all visual elements and descriptions are appealing and accurate to encourage downloads and positive user interaction.

---

## Creating a New Deployment
![Create Deployment](https://cdn.economyplus.solutions/ev6032bw.png)  
To create a new version or upload a new release of your plugin:

1. Go to the **Create Deployment** section in the dashboard.
2. Alternatively, in Visual Studio Code, you can use the Fairplay Developer extension and click **"Upload to Fairplay"**.

*Note: On the dashboard, you can view the file structure path to help with deployment management.*

Typically if you where to do this without Fairplay and wanted to send a Minecraft pack to someone else, you would; Change the UUID and Version in Manifest.json, Compress it into a .ZIP binary, and then rename it to pack.mcpack.
With Fairplay developer hub, we will take your behavior pack directly from your "Development_Behavior_Pack" folder and handle everything for you. Additonally if selected to enable obfuscation we will look at the script.entry.path(Typically index.js) and compress all files(Include import/exports) to a single file. We currently support, all ES6 Javascript webpack obfuscation modules with the exception of ShuffleStringArrays, ControlFlowFlattening, SelfDefending, DeadCodeInjection, and StringArrayRotation. 
