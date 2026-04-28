# FFXIV Translation Patch Tool
A localization tool for FFXIV. For more information, refer to the [Wiki page](https://github.com/GpointChen/FFXIVChnTextPatch-GP/wiki).

English description can be found in [Wiki pages](https://github.com/GpointChen/FFXIVChnTextPatch-GP/wiki).

Compared to the original:
1. Fixed Chinese font patch for versions after 5.5X.
2. Added functionality for localization using CSV. The CSV is output from a modified SaintCoinach.
3. Removed the part in the original exe that connects to Teemo.

## Usage
Currently, you can perform Patching using CSV, Chinese server files, or Patching override patches made by others.

To avoid issues during updates, it is recommended to restore the files before each update, then apply the Patch again after downloading the update.

When restoring, you do not need to set a folder; just click Restore.

Please note: if you haven't made additional backups of the original game files, do not apply the Patch repeatedly, as it will overwrite the backup files in the `backup` folder.

No releases to be provided for now, only source

### How to Patch Using CSV? (Recommended)
0. Download the release version on the right or compile it yourself
1. Open the EXE program
![](https://i.imgur.com/2K8CLDq.png)
2. Click ⚙
![](https://i.imgur.com/0qhqzUQ.png)
3. Select the root directory of the FFXIV game (e.g., `D:\FFXIV\SquareEnix\FINAL FANTASY XIV - A Realm Reborn`)
4. 「Translation Source」(): CSV means using the CSV files in `resource/rawexd` for Patching (recommended)
5. 「Base Language」(): Which language in the game you want to overwrite.
6. 「Text Format」
7. Click 「OK」
![](https://i.imgur.com/2K8CLDq.png)
8. Click 「Patch」

Other Patching methods are not guaranteed to be 100% usable; please refer to the [Wiki page](https://github.com/GpointChen/FFXIVChnTextPatch-GP/wiki).

## Compilation Notes
Notes on the build process can be found [here](https://hackmd.io/@GpointChen/SJi_gv-ad).

If you are using macOS, you may need to refer to [this article](https://github.com/GpointChen/FFXIVChnTextPatch-GP/blob/master/docs/MACOS_BUILD.md).  
If you are using SteamOS (on Steam Deck), you may need to refer to [this article](https://github.com/GpointChen/FFXIVChnTextPatch-GP/blob/master/docs/LINUX_BUILD.md).

## Update Notes
For details, see the project's [Wiki](https://github.com/GpointChen/FFXIVChnTextPatch-GP/wiki/1.-%E9%A6%96%E9%A0%81).

## Original Project Description

Project Description:

	This tool is used to:
	Inject CSV or Chinese resources into the international server client (SE version)

	This program
	by default only applies the Chinese font patch to the international server client,
	and does not include any Chinese content.

	This project was fully open-sourced on 2019-09-01

Usage:

	1. Download and compile the project, or directly download the release package.
	2. Extract and run the project.
	3. Select the root directory of the FFXIV game.
	4. Click the Patch button and wait.
	5. Enjoy.

	If you need Chinese content replacement,
	please copy the three files
	0a0000.win32.dat0
	0a0000.win32.index
	0a0000.win32.index2
	from the Chinese client's
	>最终幻想XIV/game/sqpack/ffxiv (FINAL FANTASY XIV/game/sqpack/ffxiv)
	folder
	to the Patching tool's
	>resource/text
	folder, then re-run the program; it will automatically read them.

	PS: This patch includes the font library content,
	so there is no need to apply the font patch again.
	PS2: Each Patching process backs up the current files,
	so avoid applying Patches on already Patched files,
	because that will back up already Patched files, causing restore rollback to fail.
	PS3: Since it is uncertain whether game updates will overwrite files,
	it is best to restore files before each update to avoid unforeseen game issues.

	Note:
	The Traditional Chinese/Classic Chinese version
	may have some bugs due to translation reasons,
	please use with caution.

	Special Note:
	This program loads Chinese resources by modifying the client.
	By using this program, you acknowledge that this is an action that violates official rules,
	and confirm that you will bear any consequences of using this program yourself.

Disclaimer:

	1. This project is for learning and technical exchange only.
	2. Any commercial use is strictly prohibited.
	3. Please delete within 24 hours after downloading.