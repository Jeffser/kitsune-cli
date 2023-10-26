# Kitsune-CLI

Kitsune-CLI is a tool that simplifies the process of creating kits for your Linux system. With Kitsune-CLI, you can package your applications and configuration files, making it effortless to replicate your setup on another computer.

⚠️ WORK IN PROGRESS: FOR TESTING PURPOSES ONLY ⚠️
## How to Use
### 1) Creating a Template

Before making a kit, you need to create a template. A template is a JSON file that defines the list of packages, directories, and commands that will be included in the kit. To create a template, use the following command:

``./kitsune make template <name:optional>``

### 2) Making a Kit

Once you have your template ready, you can proceed to create a kit. A kit is a single file that encapsulates everything needed to restore your system on another computer. To create a kit, use the following command, specifying the name of the template:

``./kitsune make kit <name of template>``

### 3) Restoring a Kit

To restore a kit on another computer, use the following command:

``./kitsune restore kit <name:optional>``

**Important:** When restoring a kit, all specified packages will be installed without a warning. Additionally, all files will be moved, potentially replacing existing ones. Please use caution when restoring a kit.

This tool is currently in development and intended for testing purposes. If you would like to contribute to its development, your help is appreciated.
Future

Our future plans for Kitsune-CLI involve creating a graphical user interface (Kitsune-GUI), potentially using technologies like GTK-4 or Qt. This GUI will provide a user-friendly experience and offer more options for managing kits.

We welcome collaboration and feedback from the community. If you have ideas or suggestions, please feel free to contribute or comment on any aspect of this project. Your input is valuable.
