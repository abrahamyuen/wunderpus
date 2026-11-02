# Wunderpus

<img src="icon.png" width="128" align="right" alt="Wunderpus icon">

Removes metadata from videos, audio and images, including AI / C2PA "Content Credentials" tags, and checks files for AI tags.

- Makes a clean **copy** next to each original: `clip.mp4` → `clip_camo.mp4`. Your originals are never changed.
- Video and audio are copied without re-encoding: no quality loss, and it's fast.
- Works on Apple Silicon and Intel Macs, macOS 13 or newer. Everything it needs is built in.

## Download

**[Download the latest Wunderpus.zip](https://github.com/abrahemp/wunderpus/releases/latest/download/Wunderpus.zip)**

## Install

1. Open your **Downloads** folder and double-click **Wunderpus.zip** to unzip it. (Safari sometimes unzips it for you.)
2. Drag **Wunderpus** into your **Applications** folder.
3. Double-click **Wunderpus** in Applications. macOS says it can't verify the developer. Click **Done**. This is expected: Wunderpus isn't registered with Apple.
4. Allow it once in System Settings:
   1. Click the **Apple menu** (top-left of the screen) → **System Settings**.
   2. In the sidebar, click **Privacy & Security**.
   3. Scroll down to **Security**. You'll see *"Wunderpus" was blocked to protect your Mac.*
   4. Click **Open Anyway**.
   5. A message asks again. Click **Open Anyway**, then enter your Mac password or use Touch ID.

   No **Open Anyway** button? It only shows for about an hour after step 3. Double-click Wunderpus again, click **Done**, and go back to Privacy & Security.
5. Wunderpus opens and sets up the right-click menu. You only do steps 3–4 once.

If **Remove Metadata** doesn't appear in Finder's right-click menu, go to **System Settings → General → Login Items & Extensions → Finder** and switch it on.

## Use

- In Finder, right-click files or folders → **Quick Actions** → **Remove Metadata**
- or drop files and folders onto the Wunderpus window or its Dock icon
- or open Wunderpus and click **Choose Files…**

**Save to** in the window puts clean copies in another folder. **Reset** goes back to saving next to the originals.

### Check for AI tags

Switch to **Check for AI Tags** at the top of the window and drop files. Checking only reads files; nothing is changed.

| Badge | Meaning |
|---|---|
| 🔺 red | AI tags found: Content Credentials, "made by AI" labels, AI tool names, AI prompts |
| ⓘ orange | No AI tags, but other details such as camera, dates, location or software |
| ✅ green | No AI tags or personal details found |

Click **Details** to see exactly which tags were found. Files with AI tags are ticked automatically. Click **Remove Metadata from Selected** to make clean copies.

## Updates

Wunderpus updates itself. Once a week, or when you click **Check for Updates**, it updates its built-in tools and its list of AI tags. When a new version of Wunderpus is out, it shows **Update Now**: one click downloads it and restarts the app.

## Limits

Wunderpus removes file metadata only. It can't detect or remove invisible watermarks embedded in the pixels themselves (e.g. SynthID). Services that recognise images by how they look can still match a cleaned copy.

## Credits

Wunderpus © 2026 Abraham Yuen. Released under the [MIT License](LICENSE).

Wunderpus includes these separate open-source tools, each under its own licence. Details, versions and source code: [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md).

- **FFmpeg**: [ffmpeg.org](https://ffmpeg.org), static macOS builds by Martin Riedl ([ffmpeg.martin-riedl.de](https://ffmpeg.martin-riedl.de)). GPL v3. Its source code is attached to every [release](https://github.com/abrahemp/wunderpus/releases).
- **ExifTool** by Phil Harvey: [exiftool.org](https://exiftool.org). Perl Artistic License / GPL.
