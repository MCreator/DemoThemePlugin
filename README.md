# Demo MCreator theme plugin

[![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/MCreator/DemoThemePlugin/blob/master/LICENSE)

This repository demonstrates some of the feature a theme plugin can do.

Some of the demo resources are re-used from the Matrix theme.

For features not demonstrated in this plugin, you can check the built-in plugins in &lt;install dir&gt;/plugins
folder of your MCreator installation for the reference.

https://mcreator.net/wiki/section/mcreator-plugins

WARNING: The plugin structure might and will change in the future so keep your eye on this repository for changes on the format if you are a plugin dev.

# Setup

In order for the plugin to work, make new file called `gradle.properties` with the following contents:

```
mcreator_path=<path to MCreator core Gradle project directory>
```

# Running MCreator with the plugin

This demo plugin comes with some Gradle tasks to help you with the development of your plugin.

* `runMCreatorWithPlugin`: Run MCreator with the plugin loaded

There is also IntelliJ IDEA run configuration for this task provided in the repository.

**Make sure to enable Java plugins in MCreator preferences, or the plugin will not be loaded.**

# Testing

We highly recommend to test your plugin by running MCreator's unit tests with your plugin loaded.

This Gradle project does this for you, you just need to run the `test` task.

There is also IntelliJ IDEA run configuration for this task provided in the repository.

Make sure to select the theme provided by this plugin in MCreator to visually check it out.

# Exporting

To export the plugin, run `jar` task and find the plugin zip file in `build/libs`.

# Installation

To install exported plugin in MCreator, put the plugin ZIP file into &lt;user home&gt;/.mcreator/plugins
or install them from MCreator's preferences window and relaunch MCreator.

# Non-plugin files

All files outside the `src/main/resources` folder are not part of the plugin structure but are there for the purpose of Intellij IDEA IDE support
for better plugin development, documentation purposes and similar.
