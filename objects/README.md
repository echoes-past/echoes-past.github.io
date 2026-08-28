# Objects Directory

This folder holds the digital objects for the Echoes of the Past collection.
The CB-CSV demo objects have been removed; see the list at the bottom of this
file for what still needs to be added.

Generally, object files should NOT be committed to your GitHub repository (as Git is not designed for binary objects and has GitHub limits the overall size of your repository).
That said, the ~120 files this project needs are small enough that keeping them
in the repository is a reasonable option — worth deciding before the first commit
of the objects.

The location of your objects is set by the "object_download", "image_small", and "image_thumb" values included in your metadata. 
Each object's location can be different, hosted in a variety of options.
For example, objects can be in a folder contained inside the project, like the demo objects (e.g. the value of "object_download" would be `/objects/demo_001.jpg`).
Or hosted in a separate web accessible location (e.g. the value of "object_download" would be `https://www.lib.uidaho.edu/digital/example/demo_001.jpg`).

Check the documentation for details of Rake tasks to process object files and how find API links.

## Files this project still needs

The paths below are already wired into `_data/echoes-past.csv` and
`_data/glossary.csv`. Download them from the project Google Drive into the
locations shown, then run `bundle exec rake generate_derivatives` to create
the `objects/small/` and `objects/thumbs/` images.

### `objects/` — 24 collection files

- `TuleLodge-River.jpg`
- `IndianAgency.jpg`
- `HallerMap.jpg`
- `FortHenrietta.jpg`
- `EchoNews.jpg`
- `EchoCityPlat.jpg`
- `KoontzBuilding.jpg`
- `Tules.jpg`
- `EchoFlood.jpg`
- `FloodErosion.jpg`
- `FloodRestoration.jpg`
- `MC-Site.jpg`
- `Fred-Hill-Sr.jpg`
- `Fred-Hill-Welcome.mp3`
- `ReflectionBooklet-River.pdf`
- `ReflectionBooklet-Rock.pdf`
- `SahaptianPhoneticPronounciationGuide.pdf`
- `UsingInquiry-Elem_Chapt4-ThinkingLikeHistorians.pdf`
- `TeachingPrimarySources_Vol2-Chap4-LocalNationalConnections.pdf`
- `M.Marker_TeachingHistoryIndigenousPerspective.pdf`
- `Exceprt_SahaptianPlaceNamesAtlas.pdf`
- `UtillaExcerpt.pdf`
- `EchoExcerpt.pdf`
- `Foldables.pdf`

### `objects/audio/` — 96 pronunciation recordings

`Sahaptian-001.mp3` through `Sahaptian-154.mp3` (not contiguous), specifically:

```
Sahaptian-001.mp3
Sahaptian-004.mp3
Sahaptian-005.mp3
Sahaptian-006.mp3
Sahaptian-007.mp3
Sahaptian-008.mp3
Sahaptian-009.mp3
Sahaptian-010.mp3
Sahaptian-013.mp3
Sahaptian-014.mp3
Sahaptian-018.mp3
Sahaptian-019.mp3
Sahaptian-020.mp3
Sahaptian-021.mp3
Sahaptian-022.mp3
Sahaptian-023.mp3
Sahaptian-024.mp3
Sahaptian-025.mp3
Sahaptian-026.mp3
Sahaptian-031.mp3
Sahaptian-032.mp3
Sahaptian-033.mp3
Sahaptian-034.mp3
Sahaptian-036.mp3
Sahaptian-037.mp3
Sahaptian-038.mp3
Sahaptian-040.mp3
Sahaptian-041.mp3
Sahaptian-042.mp3
Sahaptian-046.mp3
Sahaptian-047.mp3
Sahaptian-054.mp3
Sahaptian-057.mp3
Sahaptian-058.mp3
Sahaptian-060.mp3
Sahaptian-067.mp3
Sahaptian-068.mp3
Sahaptian-069.mp3
Sahaptian-070.mp3
Sahaptian-074.mp3
Sahaptian-075.mp3
Sahaptian-076.mp3
Sahaptian-077.mp3
Sahaptian-079.mp3
Sahaptian-080.mp3
Sahaptian-081.mp3
Sahaptian-082.mp3
Sahaptian-083.mp3
Sahaptian-084.mp3
Sahaptian-086.mp3
Sahaptian-087.mp3
Sahaptian-088.mp3
Sahaptian-089.mp3
Sahaptian-090.mp3
Sahaptian-094.mp3
Sahaptian-095.mp3
Sahaptian-096.mp3
Sahaptian-097.mp3
Sahaptian-098.mp3
Sahaptian-099.mp3
Sahaptian-100.mp3
Sahaptian-101.mp3
Sahaptian-102.mp3
Sahaptian-103.mp3
Sahaptian-104.mp3
Sahaptian-105.mp3
Sahaptian-106.mp3
Sahaptian-107.mp3
Sahaptian-108.mp3
Sahaptian-109.mp3
Sahaptian-110.mp3
Sahaptian-111.mp3
Sahaptian-112.mp3
Sahaptian-114.mp3
Sahaptian-116.mp3
Sahaptian-117.mp3
Sahaptian-118.mp3
Sahaptian-123.mp3
Sahaptian-125.mp3
Sahaptian-126.mp3
Sahaptian-127.mp3
Sahaptian-130.mp3
Sahaptian-132.mp3
Sahaptian-133.mp3
Sahaptian-135.mp3
Sahaptian-141.mp3
Sahaptian-142.mp3
Sahaptian-143.mp3
Sahaptian-144.mp3
Sahaptian-146.mp3
Sahaptian-148.mp3
Sahaptian-150.mp3
Sahaptian-151.mp3
Sahaptian-152.mp3
Sahaptian-153.mp3
Sahaptian-154.mp3
```

### `assets/img/` — interface graphics

- `HomePage.png` — the homepage banner (set in `_data/theme.yml`)
- `rock.png` — marks the standard Reflection Booklet on /printables.html
- `river.png` — marks the scaffolded Reflection Booklet on /printables.html

### Filename notes

Two filenames carry typos from the source inventory and are recorded here
exactly as spelled so they match the Drive files. If they are renamed in
Drive, update `object_location` in `_data/echoes-past.csv` to match:

- `SahaptianPhoneticPronounciationGuide.pdf` ("Pronounciation")
- `Exceprt_SahaptianPlaceNamesAtlas.pdf` ("Exceprt")
