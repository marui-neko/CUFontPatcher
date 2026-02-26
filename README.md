***

# CUFontPatcher

This plugin was created for casualties: unknown.

## What is CUFontPatcher?
**CUFontPatcher** is a BepInEx plugin that allows you to replace any in-game fonts with custom ones.
In addition to replacing fonts, you can also heavily customize the appearance of the text using the following options:

**✨ [Available Options]**
* `scale` = Font size multiplier *(1.0 = 100%)*
* `charspacing` = Spacing between characters *(Negative values shrink the spacing)*
* `linespacing` = Spacing between lines *(Negative values shrink the spacing)*
* `wordspacing` = Spacing between words *(Negative values shrink the spacing)*
* `outline` = Thickness of the text outline *(Range: 0.0 to 1.0)*
* `dilate` = Thickness of the text face/body *(Range: 0.0 to 1.0)*
* `rtl` = Right-to-Left text rendering for languages like Arabic *(Set to `true`, Default is `false`)*

> [!NOTE]
> 📝 
> A pre-compiled font asset based on **Unifont** is included in this package by default.  
> If you want to add and use your own custom fonts, you will need to create a **TextMeshPro Font Asset** using the Unity.   
> The 'Language_full.txt' file in the repository covers all the characters used in the game, so please use it when creating the font assets.

***  

## 📥 Installation

> [!TIP]
> *If you have already installed **BepInEx** and **XUnity.ResourceRedirector-BepInEx** (or XUnity.AutoTranslator-BepInEx), you can skip to **Step 3**.*

### 1. ⚙️ Installing BepInEx

1. Download `BepInEx_x64_5.x.x.zip` from the [BepInEx Releases page](https://github.com/BepInEx/BepInEx/releases).
2. Extract all contents (except `changelog.txt`) into the same folder as the game's executable (`CasualtiesUnknown.exe`).
3. Launch the game once. Once the title screen appears, close the game.
*(This step automatically generates the required folders, such as `BepInEx/plugins`.)*

### 2. 🔀 Installing XUnity.ResourceRedirector-BepInEx

1. Download `XUnity.ResourceRedirector-BepInEx.x.x.x.zip` from the [XUnity.AutoTranslator Releases page](https://github.com/bbepis/XUnity.AutoTranslator/releases).
2. Extract the contents (the `BepInEx` folder) into the same folder as the game's executable (`CasualtiesUnknown.exe`).

### 3. 🛠️ Setting Up CUFontPatcher and Fonts

1. Download `CUFontPatcher.zip` from [Here](https://github.com/marui-neko/CUFontPatcher/raw/refs/heads/main/CUFontPatcher.zip)
2. Extract the contents (the `BepInEx` folder) into the same folder as the game's executable (`CasualtiesUnknown.exe`).

#### 📁 Directory Structure
The files should be organized exactly as follows:
```ini
CasualtiesUnknown/   
└── BepInEx/   
    └── plugins/   
        └── CUFontPatcher/   
            ├── CUFontPatcher.dll    <-- The Patcher plugin   
            ├── fontmap.txt          <-- Font configuration file   
            ├── unifont_16_u_2019    <-- Your Font Asset 1   
            └── (Additional fonts)   <-- Your Font Asset 2, etc.
```
   
#### 📝 Configuring `fontmap.txt`
If you wish to customize your fonts, you can adjust the settings by editing `fontmap.txt`. For more details and examples, please refer to the comments provided within the file itself. 

***
