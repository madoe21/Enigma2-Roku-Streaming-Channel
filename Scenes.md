# Scenes

Here you can see rough drafts of the individual scenes and dialogs. Back to the [Readme.md](Readme.md).

## Scene: DetailViewScene

```bash
+---------------------------------------------+
| +-----------------------------------------+ |
| | +-------------------------------------+ | |
| | |             Favorite 1              | | |
| | | +----------+----------+-----------+ | | |
| | | | Channel 1| Channel 2| Channel 3 | | | |
| | | |   Logo   |   Logo   |   Logo    | | | |
| | | |----------+----------+-----------| | | |
| | | | Channel 4| Channel 5| Channel 6 | | | |
| | | |   Logo   |   Logo   |   Logo    | | | |
| | | +----------+----------+-----------+ | | |
| | | |             ...                 | | | |
| | | +----------+----------+-----------+ | | |
| | +-------------------------------------+ | |
| | |             Favorite 2              | | |
| | | +----------+----------+-----------+ | | |
| | | | Channel 1| Channel 2| Channel 3 | | | |
| | | |   Logo   |   Logo   |   Logo    | | | |
| | | |----------+----------+-----------| | | |
| | | | Channel 4| Channel 5| Channel 6 | | | |
| | | |   Logo   |   Logo   |   Logo    | | | |
| | | +----------+----------+-----------+ | | |
| | | |             ...                 | | | |
| | | +----------+----------+-----------+ | | |
| | +-------------------------------------+ | |
| | |             Favorite 3              | | |
| | | +----------+----------+-----------+ | | |
| | | | Channel 1| Channel 2| Channel 3 | | | |
| | | |   Logo   |   Logo   |   Logo    | | | |
| | | |----------+----------+-----------| | | |
| | | | Channel 4| Channel 5| Channel 6 | | | |
| | | |   Logo   |   Logo   |   Logo    | | | |
| | | +----------+----------+-----------+ | | |
| | | |             ...                 | | | |
| | | +----------+----------+-----------+ | | |
| | +-------------------------------------+ | |
| | |             Favorite 4              | | |
| | | +----------+----------+-----------+ | | |
| | | | Channel 1| Channel 2| Channel 3 | | | |
| | | |   Logo   |   Logo   |   Logo    | | | |
| | | |----------+----------+-----------| | | |
| | | | Channel 4| Channel 5| Channel 6 | | | |
| | | |   Logo   |   Logo   |   Logo    | | | |
| | | +----------+----------+-----------+ | | |
| | | |             ...                 | | | |
| | | +----------+----------+-----------+ | | |
| | +-------------------------------------+ | |
| +-----------------------------------------+ |
| |                Settings                 | |
| +-----------------------------------------+ |
+---------------------------------------------+
```
Description: Detail view with favorites and channels. This view will be loaded after settings are valid. Otherwise SettingsScene will be opened.

Content:
 - Vertical list with favorites.
   - For each favorite:
     - List item with favorite name.
     - Horizontal list with channels of the favorite.
       - For each channel:
         - Tile with channel name and logo.
 - Button to open the settings view.

## Scene: SettingsScene

```bash
+---------------------------------------------+
|              Settings                       |
|                                             |
|  Hostname:       [_________________]        |
|  Web Port:       [_________________]        |
|  Streaming Port: [_________________]        |
|  Username:       [_________________]        |
|  Password:       [*****************]        |
|                                             |
|  [x] Use HTTPS                              |
|  [x] Require Authentication                 |
|                                             |
|  [Cancel]    [Save]                         |
+---------------------------------------------+
```
Description: Settings view.

Content:
 - Settings menu with fields for hostname, web interface port, streaming port, username, password, and checkboxes for HTTPS and authentication.

## Dialog: DiscardChangesDialog 

```bash
+-----------------------------------------+
|        Discard Changes?                 |
|                                         |
|  Are you sure you want to discard       |
|  unsaved changes?                       |
|                                         |
|             [ No ]        [ Yes ]       |
+-----------------------------------------+
```
Description: Dialog to confirm discarding unsaved changes when leaving the SettingsScene.

Content:
 - Message informing the user about discarding unsaved changes.
 - Buttons for confirming or canceling the action.

## Scene: VideoPlayerScene

```bash
+-----------------------------------------+
|                                         |
|  [ Channel Name ]                       |
|                                         |
|  [  Video Player  ]                     |
|                                         |
|         [ Play/Pause ]                  |
|         [ Stop ]                        |
|         [  Volume Control  ]            |
+-----------------------------------------+
```
Description: Video player for playback of TV channels.

Content:
 - Video player for playback of the selected channel.
