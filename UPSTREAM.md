# Upstream

| | |
| --- | --- |
| Project | Google CTF (official archive of challenges) |
| Repository | https://github.com/google/google-ctf |
| Challenge | `2022/quals/misc-segfault-labyrinth` (Google CTF 2022) |
| Version | master (the archive has no releases) |
| Commit | 4a8f8d7808254d40f226ac2ab4604601e0e57d57 |
| Licence | Apache-2.0 |

| Here | google-ctf path |
| --- | --- |
| `app/` | [`2022/quals/misc-segfault-labyrinth`](https://github.com/google/google-ctf/tree/4a8f8d7808254d40f226ac2ab4604601e0e57d57/2022/quals/misc-segfault-labyrinth) |

The vendored folder is that commit's challenge folder, unchanged, without its Git history. The flag
is upstream's own (the `flag.txt` file the Dockerfile copies into the chroot).

`app/challenge/Dockerfile` (the challenge's own, kCTF style) builds the machine as is: `docker: { build: app/challenge }`. Its base images are pinned by tag or digest.

To update, replace the vendored folder with a newer google-ctf commit, then change this file.
