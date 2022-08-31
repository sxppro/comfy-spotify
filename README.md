# Custom Comfy Theme for Spotify ☺️️

## Inspiration

Main colours based on Spiceitfy Sleek community theme - 'Deep' 

## Preview

![Screenshot of custom Comfy theme for Spotify](media/preview.png)

## Changes
=======

**Added colour & size transitions**

![Hovering over playlist play button transitions its colour and size](media/hover.gif)

**Added translucency to playlist top bar**

![Playlist top bar with translucency](media/topbar.png)

Many quality of life changes:

* Changed background colour of progress bar
* Changed and additional 3rd colour stop to progress bar gradient
* Removed underlines on links

### ✅ Supported -> Spicetify 2.11.1, Spotify 1.1.90.
---

<<<<<<< HEAD
![Banner](media/banner.png)
=======
![Preview](https://comfy-themes.github.io/Spicetify/Comfy/preview/preview.png)
>>>>>>> upstream/main

### 📥 Automatic Installation

---

Windows -> **PowerShell**:

```powershell
iwr -useb https://raw.githubusercontent.com/NYRI4/Comfy-spicetify/main/install.ps1 | iex
```

macOS and Linux -> **Bash**:

```bash
curl -fsSL https://raw.githubusercontent.com/NYRI4/Comfy-spicetify/main/install.sh | sh
```

### 📥 Manual Installation

---

### Downloading Comfy.

CD into your `Themes` folder in `.spicetify` and run :

```sh
git clone https://github.com/Comfy-Themes/Spicetify
```

Rename the folder to `Comfy` and run these commands to apply :

```powershell
spicetify config current_theme Comfy
spicetify config color_scheme <option>
spicetify config inject_css 1 replace_colors 1 overwrite_assets 1
spicetify apply
```

### Enabling the Comfy extension.

Windows -> **Powershell**:

```powershell
cd "$(spicetify -c | Split-Path)\Themes\Comfy"
Copy-Item comfy.js ..\..\Extensions
spicetify config extensions comfy.js
spicetify apply
```

macOS and Linux -> **Bash**:

```bash
cd "$(dirname "$(spicetify -c)")/Themes/Comfy"
mkdir -p ../../Extensions
cp comfy.js ../../Extensions/.
spicetify config extensions comfy.js
spicetify apply
```

### ⚠️️ Warning

---

The theme automatically updates for users using the version of Spicetify equals or greater than `2.8.2`, however, for the users that don't want to update Spicetify to the newest version:

1. Go [here](https://comfy-themes.github.io/Spicetify/Comfy/comfy.script.js)
2. Copy the whole code (sorry for the flashbang)
3. Go into the Spicetify extension folder
4. Open the `comfy.js` file, paste the code and **save it**
5. Afterwards, in a terminal, run `spicetify apply`
6. Enjoy !

For the users that don't want to update Spicetify to the newest version, do the same with [this](https://comfy-themes.github.io/Spicetify/Comfy/app.css) and paste it in the `user.css` replacing the `@import`.

### 🖌️ Customization

---

Go into your theme folder and open either :

`color.ini` for the colors

`user.css` to modify the code
