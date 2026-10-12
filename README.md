# CrossInk setup (Xteink X4 Pro)

This is a list of one person's settings for CrossInk on an Xteink X4 Pro. It is organized menu by menu so the same setup can be recreated by hand, without copying any files.

Where the CrossInk default is known, it is listed so you can see what is different.

Edge gestures need CrossInk v1.6.1 or newer. EPUB Render Mode needs v1.3.4 or newer.

**About the asterisks (*)**: CrossInk saves many options as plain numbers. Values marked with * were turned into menu names using the order of the options in the CrossInk docs, and have not been confirmed on the device. Values without a * are plain numbers, on/off switches, or something the owner confirmed on the device.

The settings file that was read does not show when it was last saved, so a few values may be older than what the device has now.

## What is different from stock

- EPUB Render Mode is set to Light.
- Edge gestures are on: left edge changes brightness, right edge changes font size.
- Two-finger swipes are set: up/down changes warmth, left/right changes chapter.*
- Power + Up takes a screenshot.
- Pinch to resize font and two-finger rotation are both on.
- Reader font is Bookerly (from the SD card), size 18.
- Margins are 5 px on all sides.
- Paragraph alignment is "Book's Style"*, with extra paragraph spacing and forced indents on.
- Sleep screen is Custom*, using images from `/wallpapers`.
- Clock is hidden* and the time zone is UTC-3*.
- Screen refreshes every 10 pages*.

## Contents

1. Display
2. Reader
3. Controls
4. System
5. Library
6. Reading stats
7. Sleep screen
8. Fonts
9. Per-book settings
10. Step-by-step checklist
11. If you want to copy files instead
12. Things to double check

---

## 1. Display

Settings > Display

| Setting | Value | Default |
| --- | --- | --- |
| Sleep Screen | Custom* | Dark |
| Hide Battery % | Never* | Never |
| Hide Clock | Always* | |
| Refresh Frequency | Every 10 pages* | |
| UI Theme | Lyra Carousel* | |
| Sunlight Fading Fix | Off | Off |
| Dark Mode | Off | |

Frontlight (Settings > Display > Frontlight):

| Setting | Value |
| --- | --- |
| Restore Light on Wake | On |
| Frontlight Schedule | Off |

The last saved frontlight values were brightness 50 and warmth 0.

## 2. Reader

Settings > Reader. These are the global defaults for every book.

### Font

| Setting | Value | Default |
| --- | --- | --- |
| Font Family | Bookerly (SD card font) | Lexend Deca |
| Font Size | 18 (the `Bookerly_18` size) | |
| Line Spacing | 100% | |
| Word Spacing | Normal | |
| Text anti-aliasing | Off* | |

### Layout

| Setting | Value | Default |
| --- | --- | --- |
| Screen Margin (vertical) | 5 px | |
| Screen Margin (horizontal) | 5 px | |
| Paragraph Alignment | Book's Style* | Justified |
| Reading Orientation | Portrait* | Portrait |
| Hyphenation | On | |
| Extra Paragraph Spacing | On | |
| Force Paragraph Indents | On | |
| Embedded Style | On | |
| Publisher Page Numbers | Off | |
| Disable Touchscreen | Off | |

### Reading aids

Focus Reading is off and Guide Dots is off.

### Status bars

Settings > Reader > Status Bars. These apply to all books.

Each bar has seven slots: three on the left, one in the center, three on the right. In the config file the slots are stored as numbers, so the positions of the items are known but not what the items are.

- Top bar: one item, in the center slot.
- Bottom bar: three items, in the first left slot, the center slot and the second right slot.
- Percentage format: 10% (default).
- Tap to Hide Status Bar: on (default).

Open the status bar editor on your device and arrange the items the way you like (see the last section).

### EPUB Render Mode (Light)

Render mode is saved per book, so it has to be set for each book it should apply to. This setup uses Light.

Light keeps the text and basic formatting, and drops complex CSS, tables, publisher margins and indents, publisher image sizes and decorative separators. It uses the least memory.

To set it:

1. Open the book and open the reader menu (swipe up on the X4 Pro).
2. Go to the Settings tab (gear icon).
3. Pick EPUB Render Mode, then Light.

It can also be set by long-pressing an EPUB in Library or Browse Files and picking EPUB Render Mode. Changing it rebuilds that book's layout cache, but progress, bookmarks and stats are kept.

## 3. Controls

Settings > Controls

### Taps & Gestures

Settings > Controls > Taps & Gestures

| Setting | Value | Default |
| --- | --- | --- |
| Next Page | Tap & Swipe* | Tap & Swipe |
| Previous Page | Tap & Swipe* | Tap & Swipe |
| Pinch to Resize Font | On | |
| Two-finger Screen Rotation | On | On |
| Tap to Hide Status Bar | On | On |

### Edge Gestures

Settings > Controls > Taps & Gestures > Edge Gestures

| Gesture | Action | Default |
| --- | --- | --- |
| Left Edge Up | Increase Brightness | Not Set |
| Left Edge Down | Decrease Brightness | Not Set |
| Right Edge Up | Increase Font Size | Not Set |
| Right Edge Down | Decrease Font Size | Not Set |

How to use it: put one finger right at the edge of the screen and slide up or down along the edge. Brightness changes while you drag, one point at a time. Font size changes when you lift your finger. If you drift too far onto the screen, the gesture stops.

### Two-finger Swipe

Settings > Controls > Taps & Gestures > Two-finger Swipe

| Gesture | Action | Default |
| --- | --- | --- |
| Swipe Up | Increase Warmth* | Not Set |
| Swipe Down | Decrease Warmth* | Not Set |
| Swipe Left | Next Chapter* | Not Set |
| Swipe Right | Previous Chapter* | Not Set |

### Side buttons

Settings > Controls > Side Buttons

Both side buttons have custom actions (short and long press), but the action names could not be read from the config file. Orientation aware is off. See "Things to double check".

### Front buttons

Settings > Controls > Front Buttons

- Button order is the default (Back, Confirm, Left, Right).
- Remap front buttons while reading: off.
- Orientation aware: off.
- Long-press Behavior, Long-press Back action and Long-press Menu action: could not be confirmed from the config file (see the last section).

### Power button

Settings > Controls > Power Button

| Setting | Value | Default |
| --- | --- | --- |
| Short-press Action | Sleep/Wake* | Ignore |
| Long-press Action | Sleep/Wake* | Sleep/Wake |
| Power + Up | Take Screenshot | Off |

### Home button

Settings > Controls > Home Button

The Home button works while reading. The tap, double tap and long press actions were changed, but the action names could not be read (see the last section).

## 4. System

Settings > System

| Setting | Value |
| --- | --- |
| Time to Sleep | 5 minutes |
| Custom Boot Screen | On (default) |
| Time zone (Device > UTC offset) | UTC-3* |
| Language | English |
| Show hidden files | Off |
| Hide file extensions | Off |
| Move finished books to Read folder | Off |
| Remove read books from Recents | Off |

## 5. Library

Sort is on the Library screen itself (the Left button, or the sort control at the top on touch). The rest is in Library > Settings.

| Setting | Value |
| --- | --- |
| Sort | Recently Opened, descending* |
| Use Book Metadata | On |
| Rows | Expanded* |
| Recently Opened View | List* |
| Show Series | On |
| Show Genre | On |
| Formats shown | EPUB, XTC, TXT and Markdown (all on) |
| Hide finished books | Off |

## 6. Reading stats

Settings > System > Reading Stats

- Track Reading Stats: on.
- Automatic backup of all-time stats: on. Backups are saved in `.crossink-stats-backup/`. The exact menu label may be different.

## 7. Sleep screen

- Sleep Screen is set to Custom*.
- The images are in the `/wallpapers` folder on the SD card, and that folder is saved as the preferred sleep folder.
- Use BMP files, 480 x 800 px (the X4 screen size). Uncompressed BMP works best.
- The firmware remembers the last few images it showed so it does not repeat them right away.

The docs that were reviewed do not say where the preferred sleep folder is chosen on the device, so the exact menu for it is not known. They only mention `/.sleep` and `/sleep` as sleep image folders.

## 8. Fonts

Fonts are `.cpfont` files inside `/.fonts/<FontName>/`.

| Font | Sizes installed | In use |
| --- | --- | --- |
| Bookerly | 14, 18, 24, 32 | Yes |
| Monocraft | 16, 18, 24, 32 | No |

```
/.fonts/
  Bookerly/
    Bookerly_14.cpfont
    Bookerly_18.cpfont
    Bookerly_24.cpfont
    Bookerly_32.cpfont
  Monocraft/
    Monocraft_16.cpfont
    Monocraft_18.cpfont
    Monocraft_24.cpfont
    Monocraft_32.cpfont
```

Fonts can be downloaded from Settings > Reader > Font Options > Manage Fonts (over Wi-Fi), or `.cpfont` files can be taken from https://inky.crossink.dev/#downloads and put in `/.fonts/`. It is not known whether Bookerly is available there. If it is not, any font can be used with the other values kept the same.

## 9. Per-book settings

Some settings are saved per book and take priority over the global ones. This comes from the cache folders on the owner's card. The render mode is clear (those books have `_light` layout files), but the font sizes come from a binary file that was decoded by guessing, so treat them as approximate.

| Book | Render mode | Font size |
| --- | --- | --- |
| 23 minutos | Light | 14 |
| Fahrenheit 451 | Light | 14 |
| 1984 | no layout cache on the card | 14 |
| Ainda Estou Aqui | no layout cache on the card | 24 |
| Blade Runner | no per-book settings | global (18) |

To remove a book's own settings, long-press it in Library or Browse Files and choose Reset Book Reader Settings.

## 10. Step-by-step checklist

To get the same setup quickly, go through this list.

Settings > Display
- [ ] Sleep Screen: Custom
- [ ] Hide Clock: Always
- [ ] Refresh Frequency: 10 pages
- [ ] UI Theme: Lyra Carousel
- [ ] Frontlight > Restore Light on Wake: On

Settings > Reader
- [ ] Font Options > Font Family: Bookerly, size 18
- [ ] Line Spacing: 100%
- [ ] Margins: 5 and 5
- [ ] Paragraph Alignment: Book's Style
- [ ] Hyphenation: On
- [ ] Extra Paragraph Spacing: On
- [ ] Force Paragraph Indents: On
- [ ] Focus Reading and Guide Dots: Off
- [ ] Status Bars: one item on top (center), three on the bottom

Settings > Controls > Taps & Gestures
- [ ] Pinch to Resize Font: On
- [ ] Two-finger Screen Rotation: On
- [ ] Edge Gestures, Left Up: Increase Brightness
- [ ] Edge Gestures, Left Down: Decrease Brightness
- [ ] Edge Gestures, Right Up: Increase Font Size
- [ ] Edge Gestures, Right Down: Decrease Font Size
- [ ] Two-finger Swipe, Up: Increase Warmth
- [ ] Two-finger Swipe, Down: Decrease Warmth
- [ ] Two-finger Swipe, Left: Next Chapter
- [ ] Two-finger Swipe, Right: Previous Chapter

Settings > Controls > Power Button
- [ ] Short-press Action: Sleep/Wake
- [ ] Power + Up: Take Screenshot

Settings > System
- [ ] Time to Sleep: 5 minutes
- [ ] Device > UTC offset: UTC-3
- [ ] Reading Stats: tracking On, automatic backup On

Library
- [ ] Sort: Recently Opened, descending

For each book it should apply to
- [ ] Reader menu > Settings tab > EPUB Render Mode: Light

On the SD card
- [ ] Fonts in `/.fonts/`
- [ ] BMP wallpapers (480 x 800) in `/wallpapers`

## 11. If you want to copy files instead

| Path | What it is | Copy? |
| --- | --- | --- |
| `.crosspoint/crossink-settings.json` | The CrossInk settings (this is the file that was read for this README) | Yes |
| `.crosspoint/state.json` | Sleep folder and last opened book | Optional |
| `.fonts/` | Bookerly and Monocraft | Yes |
| `.crosspoint/epub_*/reader_settings.bin` | Per-book settings. The folder name comes from the book path, so it only works for the same file path | Optional |
| `.crosspoint/settings.json` | An older-format settings file with different values, probably a leftover | No |
| `.crosspoint/wifi.json` | Saved Wi-Fi networks and passwords | No, do not share this one |
| `.crossink-stats-backup/` | Reading stats backups | Optional |

## 12. Things to double check

These could not be matched to menu names, or they are the values most likely to be wrong:

- Side buttons: Left/Up short = 31, long = 68. Right/Down short = 2, long = 69.
- Home button: tap = 23, double tap = 25, long press = 24.
- Front buttons: Long-press Behavior = 2, Long-press Back action = 16, Long-press Menu action = 0.
- Status bar items: top slots `[0,0,0,8,0,0,0]`, bottom slots `[9,0,0,4,0,7,0]`. The numbers are item IDs, and it is not known which item each one is.
- Images (Settings > Reader): stored as 1.
- EPUB Indexing Method: stored as 0.
- Reading stats idle threshold: stored as 30.
- Sleep screen cover mode: stored as the second option, which is probably Crop (only matters when Cover is used as the sleep screen).
- UI Theme: stored as 4, which was read as Lyra Carousel. The card also has `home_carousel_cache_*` files, which supports that.
- Power + Up: the config file says 0, but on the device it is set to Take Screenshot. That shows a decoded number can be wrong, so the same could be true for any value marked with *.
- Other raw values in the config: `swapLibraryFileBrowser` = 1, `uiScale` = 1, `sdFontSizeRange` = 2.
