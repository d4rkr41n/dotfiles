# First, Ubernut
### Setup
Install zsh    
`sudo apt install zsh`

Install oh-my-zsh    
`sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"`

Install PowerLevel10K Theme    
`git clone https://github.com/romkatv/powerlevel10k.git $ZSH_CUSTOM/themes/powerlevel10k
`
Install suggestions and syntax highlighting    
```
git clone https://github.com/zsh-users/zsh-autosuggestions.git $ZSH_CUSTOM/plugins/zsh-autosuggestions
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git $ZSH_CUSTOM/plugins/zsh-syntax-highlighting
```

Now open ~/.zshrc and make these edits...    
`ZSH_THEME="powerlevel10k/powerlevel10k"`    
and near the bottom..    
`plugins=(git zsh-autosuggestions zsh-syntax-highlighting)`

### Theme
```
"colorScheme":  "Custurd",
"hidden": false,
"acrylicOpacity": 0.9,
"closeOnExit": true,
"cursorColor": "#FFFFFF",
"cursorHeight": 25,
"cursorShape": "vintage",
"fontFace": "MesloLGS NF",
"fontSize": 13,
"padding": "0, 0, 0, 0",
"snapOnInput": true,
"useAcrylic": true,
"startingDirectory": "%USERPROFILE%"
```
WITH
```
{
    "name": "Custurd",
    "cursorColor": "#F8F8F2",
    "selectionBackground": "#44475A",
    "background": "#16171D",
    "foreground": "#F8F8F2",
    "black": "#3C3744",
    "blue": "#BD93F9",
    "cyan": "#A0C1B9",
    "green": "#b74c4c",
    "purple": "#994876",
    "red": "#FF5555",
    "white": "#F8F8F2",
    "yellow": "#F1FA8C",
    "brightBlack": "#E373C8",
    "brightBlue": "#D6ACFF",
    "brightCyan": "#70A0AF",
    "brightGreen": "#69FF94",
    "brightPurple": "#FF92DF",
    "brightRed": "#D36135",
    "brightWhite": "#FFFFFF",
    "brightYellow": "#E6AA68"
}
```

# Now, Winderrs
### Setup
Install Oh-My-Posh Modules    
```
Install-Module posh-git -Scope CurrentUser
Install-Module oh-my-posh -Scope CurrentUser
```

Install Powerline Fonts (This will take a while)    
```
git clone https://github.com/powerline/fonts.git --depth=1
cd .\fonts\
.\install.ps1
```

Open profile    
`notepad $PROFILE`

Add these lines    
```
Import-Module posh-git
Import-Module oh-my-posh
Set-PoshPrompt Paradox
```

### Theme
I just use dracula for now (Or just don't really set it up) because I actually don't like to use powershell.

```
"colorScheme":  "Dracula",
"acrylicOpacity": 0.9,
"closeOnExit": true,
"cursorColor": "#FFFFFF",
"cursorShape": "bar",
"fontFace": "Meslo LG S for Powerline",
"fontSize": 13,
"hidden": false,
"padding": "0, 0, 0, 0",
"snapOnInput": true,
"startingDirectory": "%USERPROFILE%",
"useAcrylic": true
```

Colors...
```
{
  "name": "Dracula",
  "cursorColor": "#F8F8F2",
  "selectionBackground": "#44475A",
  "background": "#282A36",
  "foreground": "#F8F8F2",
  "black": "#21222C",
  "blue": "#BD93F9",
  "cyan": "#8BE9FD",
  "green": "#50FA7B",
  "purple": "#FF79C6",
  "red": "#FF5555",
  "white": "#F8F8F2",
  "yellow": "#F1FA8C",
  "brightBlack": "#6272A4",
  "brightBlue": "#D6ACFF",
  "brightCyan": "#A4FFFF",
  "brightGreen": "#69FF94",
  "brightPurple": "#FF92DF",
  "brightRed": "#FF6E6E",
  "brightWhite": "#FFFFFF",
  "brightYellow": "#FFFFA5"
}
```
