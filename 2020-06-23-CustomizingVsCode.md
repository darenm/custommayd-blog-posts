# Customizing the Visual Studio Code Integrated Terminal

I continually forget how to customize the integrated terminal in VSCode, so I will capture it here for posterity.

## Configure default PowerShell version

Before configuring Shell Launcher, I want to set PowerShell Core as the default PowerShell version. To do so, open up the VS Code user settings.json file by clicking on **file > preferences > settings, select ...** and then **Open settings.json**.

Modify the settings.json file to include terminal.integrated.shell.windows. The update must be well formed json. If you have other settings in your settings.json file, you may need to adjust the following example.

```json
{
    "terminal.integrated.shell.windows": "c:/Program Files/PowerShell/7/pwsh.exe"
}
```

## Change Terminal Colors
Open user settings, switch to JSON and add something similar to:

```json
"workbench.colorCustomizations": {
  "terminal.background":"#FEFBEC",
  "terminal.foreground":"#6E6B5E",
  ...
}
```

Check <https://glitchbone.github.io/vscode-base16-term> for some presets.
