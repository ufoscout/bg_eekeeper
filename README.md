# bg_eekeeper

This repository contains copies of the source code shipped by the upstream
[EE Keeper SourceForge project](https://sourceforge.net/projects/eekeeper),
a saved-game editor for the *Baldur's Gate* family of games:

- `shadow-keeper/` — the original **Shadow Keeper** source.
- `eekeeper-qt/` — **EE Keeper - Qt**, a Qt-based port/successor of Shadow
  Keeper targeting the Enhanced Edition releases.
- `translations/` — localization resource projects for EE Keeper (English,
  French, Hebrew, Italian, Korean, Brazilian Portuguese, Simplified Chinese).

## `shadow-keeper/`

**Shadow Keeper** is the original saved-game editor for *Baldur's Gate II:
Shadows of Amn* (and *Throne of Bhaal*), released in 2000 by Aaron O'Neil. It
is a Windows/MFC C++ application that lets users edit characters, items, and
party state in BG2 save games. It is the ancestor of EE Keeper.

Source:

- Project page: https://sourceforge.net/projects/eekeeper
- SVN repository: https://svn.code.sf.net/p/eekeeper/shadowkeeper/
- Revision imported: r1 (2015-02-01), the latest available at the time of
  import

To refresh from upstream:

```sh
svn checkout https://svn.code.sf.net/p/eekeeper/shadowkeeper/ shadow-keeper
```

License: Copyright (c) 2000 Aaron O'Neil, BSD-style license (see
`eekeeper-qt/ShadowKeeper/COPYING` for the full text — the upstream
`shadowkeeper/` tree does not ship a `COPYING` file of its own).

## `eekeeper-qt/`

**EE Keeper - Qt** is the Qt port of EE Keeper, itself the spiritual successor
to Shadow Keeper for *Baldur's Gate: Enhanced Edition* and *Baldur's Gate II:
Enhanced Edition*. It uses the Qt 5 toolkit to render its GUI, with the goal
of providing a cross-platform alternative to the original Windows-only
EE Keeper.

Source:

- Project page: https://sourceforge.net/projects/eekeeper
- SVN repository: https://svn.code.sf.net/p/eekeeper/eekeeper-qt/
- Revision imported: r3 (2015-02-01), the latest available at the time of
  import

To refresh from upstream:

```sh
svn checkout https://svn.code.sf.net/p/eekeeper/eekeeper-qt/ eekeeper-qt
```

Authors: primarily Marshall Mattingly and Troodon80. Distributed under a
3-clause BSD-style license (see `eekeeper-qt/COPYING`). Incorporates code from
Shadow Keeper (Copyright (C) 2000 Aaron O'Neil — see
`eekeeper-qt/ShadowKeeper/COPYING`) and uses the Qt Toolkit (see
`eekeeper-qt/Qt/COPYING`).

## `translations/`

EE Keeper's localization projects. This is a Visual Studio solution
(`eekeeper-translations.sln`) containing one resource-DLL subproject per
supported language. Each locale subfolder (`en-US/`, `fr-FR/`, `he-IL/`,
`it-IT/`, `ko-KR/`, `pt-BR/`, `zh-CN/`) holds a translated `EEKeeper.rc`
resource script plus its accompanying `.vcxproj` and `res/` assets. These are
the source files used to build the per-language resource DLLs shipped by
EE Keeper.

Source:

- Project page: https://sourceforge.net/projects/eekeeper
- SVN repository: https://svn.code.sf.net/p/eekeeper/translations/
- Revision imported: r11 (2017-06-14), the latest available at the time of
  import

To refresh from upstream:

```sh
svn checkout https://svn.code.sf.net/p/eekeeper/translations/ translations
```
