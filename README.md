<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif">

# 🎮 Minecraft Skin Pack Builder
<p><img src="https://komarev.com/ghpvc/?username=abdurrahman101bd" alt="Profile Views"> <img src="https://custom-icon-badges.herokuapp.com/badge/Repo-blue.svg?logo=repo" alt="Repository Count Badge">
<img src="https://custom-icon-badges.herokuapp.com/badge/Star-yellow.svg?logo=star" alt="Stars Badge">
<img src="https://custom-icon-badges.herokuapp.com/badge/Issue-red.svg?logo=issue" alt="Issue Badge">
<img src="https://custom-icon-badges.herokuapp.com/badge/Fork-orange.svg?logo=fork" alt="Fork Badge">
<img src="https://custom-icon-badges.herokuapp.com/badge/Commit-green.svg?logo=commit" alt="Commit Badge">
<img src="https://custom-icon-badges.herokuapp.com/badge/Pull Request-purple.svg?logo=pr" alt="Pull Badge"></p>

![License](https://img.shields.io/badge/License-MIT-blue.svg)
![GitHub last commit](https://img.shields.io/github/last-commit/abdurrahman101bd/minecraft-skin-pack-builder)
![GitHub issues](https://img.shields.io/github/issues-raw/abdurrahman101bd/minecraft-skin-pack-builder)
![GitHub stars](https://img.shields.io/github/stars/abdurrahman101bd/minecraft-skin-pack-builder?style=social)
![GitHub forks](https://img.shields.io/github/forks/abdurrahman101bd/minecraft-skin-pack-builder?style=social)
![GitHub repo size](https://img.shields.io/github/repo-size/abdurrahman101bd/minecraft-skin-pack-builder)
![GitHub issues](https://img.shields.io/github/issues/abdurrahman101bd/minecraft-skin-pack-builder)
![GitHub pull requests](https://img.shields.io/github/issues-pr/abdurrahman101bd/minecraft-skin-pack-builder)

![Version](https://img.shields.io/badge/Version-1.0-blue)

---

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)


<div align="center">

![Minecraft](https://img.shields.io/badge/Minecraft-Bedrock%20Edition-62B47A?style=for-the-badge&logo=minecraft&logoColor=white)
![HTML](https://img.shields.io/badge/HTML5-Single%20File-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge)
![No Install](https://img.shields.io/badge/No%20Install-Required-blue?style=for-the-badge)

**Create Minecraft Bedrock `.mcpack` skin packs directly in your browser — no software needed.**

[🚀 Live Demo](https://abdurrahman101bd.github.io/minecraft-skin-pack-builder) · [📦 Download](https://github.com/abdurrahman101bd/minecraft-skin-pack-builder/blob/main/index.html) · [🐛 Report Bug](https://github.com/abdurrahman101bd/minecraft-skin-pack-builder/issues)

</div>

---

## ✨ Features

- **Drag & Drop** — Drop multiple PNG skin files at once
- **ZIP Import** — Load skins from an existing `.zip` archive
- **3D Preview** — Real-time animated 3D model viewer (Walk / Run / Idle)
- **16 Backgrounds** — Minecraft-themed backgrounds for the preview (Nether, The End, Overworld, Aurora, and more)
- **Rename Skins** — Edit the display name of each skin before exporting
- **Direct `.mcpack` Export** — Builds a proper Bedrock-compatible skin pack, no extra steps
- **Zero Dependencies** — Single HTML file, runs entirely in the browser

---

## 📸 Preview

> *Import skins → Preview in 3D → Build & Download*

<div align="center">

| Import | 3D Preview | Export |
|--------|-----------|--------|
| Drag & Drop PNG / ZIP | Animated model viewer | One-click `.mcpack` |

</div>

---

## 🚀 How to Use

**1. Open the tool**
- Download `index.html` and open it in any modern browser
- Or visit
- [![Live Demo](https://img.shields.io/badge/Live%20Demo-Click%20Here-brightgreen?style=for-the-badge&logo=google-chrome)](https://abdurrahman101bd.github.io/minecraft-skin-pack-builder)

---

**2. Import your skins**
- Drag and drop `.png` skin files onto the drop zone
- Or click the drop zone to browse files
- Or use **"Load from .zip Archive"** to import multiple skins at once

> ⚠️ Skins must be PNG format — `64×64` (Java/Bedrock) or `64×32` (Legacy)

**3. Customize**
- Click any skin in the library to preview it in 3D
- Edit the name field under each skin (this is the in-game display name)
- Switch animations: **Walk**, **Run**, or **Idle**
- Click 🎨 to change the preview background

**4. Export**
- Enter a **Pack Name** in the Pack Config section
- Click **▼ BUILD .MCPACK**
- The file downloads automatically

**5. Install on Minecraft Bedrock**
- On **Windows**: Double-click the `.mcpack` file — Minecraft opens and imports it
- On **Android**: Open the file with Minecraft from your file manager
- On **iOS**: Use the Share menu → Open with Minecraft

---

## 📁 Generated Pack Structure

```
MySkinPack.mcpack
├── manifest.json        # Pack metadata & UUID
├── skins.json           # Skin definitions
├── skin1.png
├── skin2.png
├── ...
└── texts/
    ├── en_US.lang       # Display names
    └── languages.json
```

---

## 🛠️ Tech Stack

| Library | Purpose |
|---------|---------|
| [skinview3d](https://github.com/bs-community/skinview3d) | 3D skin model renderer (Three.js based) |
| [JSZip](https://stuk.github.io/jszip/) | ZIP/MCPACK file generation |
| [Press Start 2P](https://fonts.google.com/specimen/Press+Start+2P) | Pixel font (Google Fonts) |

No frameworks. No build tools. Just one `.html` file.

---

## ⚠️ Known Limitations

- Skin geometry is set to `geometry.humanoid.customSlim` (slim arms) for all skins
- All skins export as `type: "free"` — paid/locked skin packs are not supported

---

## 🤝 Contributing

Pull requests are welcome! For major changes, please open an issue first.

```bash
git clone https://github.com/abdurrahman101bd/minecraft-skin-pack-builder.git
cd minecraft-skin-pack-builder
# Just open index.html in a browser — no build step needed
```

---

## 📝 License

This project is licensed under the MIT License - see the [MIT License](LICENSE) file for details.

---

## 👥 Authors

**Abdur Rahman**

[![GitHub](https://img.shields.io/badge/GitHub-Profile-181717?style=for-the-badge&logo=github)](https://github.com/abdurrahman101bd)
[![Gmail](https://img.shields.io/badge/Email-abdurrahman101bd@gmail.com-red?style=for-the-badge&logo=gmail&logoColor=white)](mailto:abdurrahman101bd@gmail.com)

---

## 📞 Contact

[![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/abdurrahman101bd)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/abdurrahman101bd)
[![Twitter](https://img.shields.io/badge/Twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white)](https://x.com/abdurrahman101b)
[![Facebook](https://img.shields.io/badge/Facebook-1877F2?style=for-the-badge&logo=facebook&logoColor=white)](https://www.facebook.com/abdurrahman101bd)

---

## 🌟 Star History

If you find this project useful, please consider giving it a star ⭐

[![Star History Chart](https://api.star-history.com/svg?repos=abdurrahman101bd/minecraft-skin-pack-builder&type=Date)](https://star-history.com/#abdurrahman101bd/minecraft-skin-pack-builder&Date)

---

<p align="center">
  Made with ❤️ by <a href="https://github.com/abdurrahman101bd">Abdur Rahman</a>
</p>

<p align="center">
  <a href="#-minecraft-skin-pack-builder">Back to Top ⬆️</a>
</p>

<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif">
