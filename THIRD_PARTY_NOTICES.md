# Third-Party Notices

Wunderpus © 2026 Abraham Yuen. Wunderpus's own code is released under the MIT License (see [LICENSE](LICENSE); a copy is inside the app at `Wunderpus.app/Contents/Resources/LICENSE`).

Wunderpus includes the open-source tools listed below. They are **separate programs** that Wunderpus runs as-is: they are not modified and not compiled into Wunderpus's own code. Each one stays under its own licence, summarised below. Copies of these notices and of the licence texts are inside the app at `Wunderpus.app/Contents/Resources/`.

Versions listed are the ones bundled in this release. Wunderpus's built-in updater may later download newer versions of these tools from the same sources, under the same licences.

---

## FFmpeg

Used to remove metadata from video and audio files without re-encoding.

| | |
|---|---|
| **Bundled as** | `Wunderpus.app/Contents/Resources/bin/ffmpeg-arm64` and `ffmpeg-x86_64` |
| **Version** | 9.0.2 (static macOS builds by Martin Riedl, https://ffmpeg.martin-riedl.de) |
| **Copyright** | © 2000–2026 the FFmpeg developers |
| **Licence** | GNU General Public License, **version 3** or (at your option) any later version. These builds are configured with `--enable-gpl --enable-version3` and include external libraries that are themselves under the GPL (such as x264 and x265), so the binaries as a whole are GPL v3. |
| **Licence text** | `Wunderpus.app/Contents/Resources/licenses/GPL-3.0.txt` · https://www.gnu.org/licenses/gpl-3.0.html |
| **Project** | https://ffmpeg.org |

**Source code.** The complete FFmpeg 9.0.2 source code is attached to each Wunderpus release on GitHub (`ffmpeg-9.0.2.tar.xz`, under *Assets*: https://github.com/abrahamyuen/wunderpus/releases) and is also available from https://ffmpeg.org/releases/ffmpeg-9.0.2.tar.xz. The build configuration and the external libraries compiled into the binaries are listed by running `ffmpeg -version` and are documented, with their build scripts, at https://ffmpeg.martin-riedl.de. Those libraries remain under their own open-source licences.

FFmpeg is a trademark of Fabrice Bellard, originator of the FFmpeg project. Wunderpus is not affiliated with or endorsed by the FFmpeg project.

---

## ExifTool

Used to read and remove metadata (EXIF, XMP, IPTC, C2PA and more) from images, and to check files for AI tags.

| | |
|---|---|
| **Bundled as** | `Wunderpus.app/Contents/Resources/exiftool/` (complete Perl source code) |
| **Version** | 13.60 |
| **Copyright** | © 2003–2026 Phil Harvey |
| **Licence** | Free software; you can redistribute it and/or modify it under the same terms as Perl itself: the Artistic License or the GNU General Public License, version 1 or later |
| **Licence text** | https://dev.perl.org/licenses/ · GPL v3 (a later version of the GPL, which this licence allows) is included at `Wunderpus.app/Contents/Resources/licenses/GPL-3.0.txt` |
| **Project & source** | https://exiftool.org (the bundled copy is itself the full source) |

Wunderpus is not affiliated with or endorsed by ExifTool or Phil Harvey.

---

## Getting the source code

If you can't get the source code for any bundled component from the links above, open an issue at https://github.com/abrahamyuen/wunderpus/issues and it will be provided free of charge. This offer is valid for at least three years after the last release that included that component.
