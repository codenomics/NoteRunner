# NoteRunner

> This application is built by AI. I made this for myself and I'm uploading it to GitHub for backup and to share in case anyone can get any use out of it. It's pretty specific to my setup and my needs, but if you can get any use out of it, then enjoy.
>
> Use at your own risk. I offer no warranty or guarantees for this software.

## Download

**Latest version: v1.7** (Oct 8, 2026)

- [NoteRunner_v1.7_no-install.zip](https://github.com/codenomics/NoteRunner/releases/download/v1.7/NoteRunner_v1.7_no-install.zip) - 138 KB
- [NoteRunner_v1.7_Setup.exe](https://github.com/codenomics/NoteRunner/releases/download/v1.7/NoteRunner_v1.7_Setup.exe) - 211 KB
- [NoteRunner_v1.7_source.zip](https://github.com/codenomics/NoteRunner/releases/download/v1.7/NoteRunner_v1.7_source.zip) - 130 KB

What's new in v1.7:

- updater versioning fix**

Older versions are on the [Releases page](https://github.com/codenomics/NoteRunner/releases).

## Getting started

### Installer (recommended)

1. Download the file ending in `_Setup.exe` above.
2. Double-click it and click Install. It installs just for you - no admin password needed - and adds Start menu and Desktop shortcuts.
3. To remove it later: Windows Settings > Apps, find NoteRunner and click Uninstall.

### No install (portable zip)

1. Download the file ending in `_no-install.zip` above.
2. Right-click it > Extract All, and pick a folder. Don't run it from inside the zip.
3. Open the folder and double-click the app's .exe. Nothing is installed; delete the folder to remove it.

Windows says "Windows protected your PC"? Click More info > Run anyway. It shows that for apps without a paid signing certificate.

## Source code

Want to see how it works, or build it yourself? Download the file ending in `_source.zip` above, extract it and double-click `Build.bat`. It only uses the C# compiler that already comes with Windows, so there is nothing to install.

## More details

```
NOTERUNNER
==========

A notes and outlines app. Documents live in folders in the sidebar. Each
document is a list of bullets: Tab tucks a line under the one above, and
clicking a bullet folds away the lines under it.


GETTING STARTED
---------------
Pick one. Both give you the same app.

OPTION 1 - INSTALLER (recommended)
  Download the file ending in _Setup.exe, double-click it and click Install.
  It installs just for you (no admin password) and adds Start menu and
  Desktop shortcuts. Needs Windows 10 or 11 (64-bit).
  To remove it later: Windows Settings > Apps > NoteRunner > Uninstall.

OPTION 2 - NO INSTALL (zip)
  1. Download the file ending in _no-install.zip. Right-click it -> Extract
  All... and put the NoteRunner folder somewhere it can stay (for example
  Documents). Don't run it from inside the zip.
  2. Double-click NoteRunner.exe. Nothing is installed; to remove it, delete
  the folder.

EITHER WAY
  Optional: pin it to Start (right-click it in the Start menu or on the
  desktop -> Pin to Start).

"Windows protected your PC"? Click "More info" -> "Run anyway".
Windows shows that for apps downloaded from the internet that aren't
signed with a paid certificate.


USING IT
--------
Sidebar
- + Doc makes a new document, + Folder a new folder (Ctrl+N / Ctrl+Shift+N).
- Drag documents and folders to sort them. Drop one onto a folder to put it
  inside. Drag the line between the sidebar and the page to make it wider.
- Double-click (or F2) to rename. Right-click for rename, new, copy as
  text and delete.
- Deleted documents and folders go to Recently deleted (bottom of the
  sidebar) for 30 days. Ctrl+Z in the sidebar brings the last one straight back.
  Recently deleted > From a daily backup... copies a document back out of the
  daily backups.
- The search box at the top searches every document (Ctrl+F). Press Enter to
  jump to each match in turn (Shift+Enter goes back); the current one glows.

Writing
- Enter = new line.  Shift+Enter = line break inside the same bullet.
- Tab = tuck the line under the one above.  Shift+Tab = move it back out.
- Click a bullet to fold / unfold the lines under it. A bullet with a ring
  around it has folded lines inside.
- Drag a bullet to move that line and everything under it.
- Ctrl+Shift+Up / Down moves a line.  Ctrl+Enter crosses it off.
- Shift+Up / Shift+Down (or dragging across lines) selects whole lines.
  Then Tab, Shift+Tab, Delete, Ctrl+C, Ctrl+X and Ctrl+Enter work on all of them.
- Ctrl+Z / Ctrl+Y undo and redo.
- Pasting several lines makes each one its own bullet (indents are kept).
- Ctrl+A selects the line's text; keep pressing it to select the line, then
  one level up each time, until the whole document is selected.

Formatting
- Right-click a line for Heading (3 sizes) and Color label (6 colors).
  Shortcuts: Ctrl+Shift+H (heading), Ctrl+Shift+L or Ctrl+Shift+1-6 (color,
  Ctrl+Shift+0 removes it).
- **bold**, __italic__, ~~crossed out~~, `code` and [links](https://...) show
  formatted when you're not typing in the line. Ctrl+B / Ctrl+I / Ctrl+` add them.
- A line starting with ` ` ` is a code block. Web addresses are clickable.
- F1 or the Keys button shows every shortcut.
- Hide crossed off (top right) hides the lines you've crossed off; click
  Show crossed off to bring them back.
- The panel button at the top left (or Ctrl+\) hides and shows the sidebar.
- Misspelled words get a red squiggle. Right-click one for suggestions.

It saves by itself as you type.


SHARING A FOLDER AS FILES
-------------------------
Right-click a folder > Share as files, then pick where the files go: the
standard place (a Shared folder next to your notes) or any folder you choose.
Its documents are then also kept there as plain text files (one per document).
Right-click > Change where the files go... moves them somewhere else later.
Changes in NoteRunner are written there, and changes made to those files come
back into NoteRunner by themselves - handy for working on notes with other
tools. The READ ME in the Shared folder explains the layout. Right-click >
Stop sharing as files moves the copies into Backups (your documents stay).


SECURE FOLDERS
--------------
Right-click a folder > Make secure... and what's inside is saved scrambled
instead of as plain text (in the same notes.txt, so it syncs like the rest).
You can add a password: then the folder starts locked each time NoteRunner
opens - click it and type the password to open it, or right-click > Lock now.
Without a password it just isn't readable as plain text.
If you forget the password, there's no way to get those notes back.
Secure folders can't also be shared as files.


TEMPLATES
---------
Right-click a document > Save as template to copy it into the Templates
folder. Then use the template icon at the top of the sidebar (or right-click >
New from template) to start a new document from it. In a template, {date},
{time} and {weekday} are filled in when the new document is made.


SETTINGS
--------
Click Settings (top right) for:
- Theme: Synthwave, Dark or Light
- Layout: Normal, or Compact for less space between lines
- Text size: Small, Normal, Large or Larger
- Page: line the notes up on the Left, Center or Right
- Spell check on or off (needs Windows 8 or newer)
- Notes folder (and Google Drive) and Import from Dynalist
- Update check: At startup (default) or Off, and a button to check now


MOVING OVER FROM DYNALIST
-------------------------
Click Settings > Import from Dynalist and follow the steps. It copies all your
folders and documents, with headings, color labels, crossed-off lines and notes.
Dynalist notes become an extra line inside their bullet.


SYNCING WITH GOOGLE DRIVE
-------------------------
All notes are kept in one file, notes.txt, in the notes folder
(Documents\NoteRunner to start with).

1. Install Google Drive for desktop (free) and sign in.
2. In NoteRunner click Settings > Notes folder Change... -> Use Google Drive.
   Your notes move to My Drive\NoteRunner and sync online by themselves.
3. On another PC: install Google Drive and NoteRunner, click Settings >
   Notes folder Change... -> Use Google Drive, and pick "Open those notes".

If the notes file is changed on another PC, NoteRunner loads the new version
by itself. Avoid typing on two PCs at the same moment - if both change it,
the other version is kept in the Backups folder so nothing is lost.


GOOD TO KNOW
------------
- A copy of your notes is kept each day in the Backups folder next to
  notes.txt (the newest 30 days).
- Settings are kept in %APPDATA%\NoteRunner\settings.txt.
- Updates: when NoteRunner starts it checks GitHub for a newer version (it only
  reads the public release page; nothing is sent). If there is one it asks
  whether to update. With the installer, Update now saves your notes, downloads
  the new installer and runs it; with the no-install zip, it opens the download
  page. Settings > Update check turns the startup check off, and the Settings
  button checks on demand.
- If something goes wrong, NoteRunner-log.txt next to NoteRunner.exe says what.
- To remove NoteRunner: delete its folder, plus %APPDATA%\NoteRunner.
  Your notes stay in the notes folder until you delete that too.
```

