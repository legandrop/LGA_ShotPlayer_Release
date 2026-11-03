# What's new in LGA Shot Player

## v1.002 (2026-11-03)

- **New:** Podés marcar los cortes de un EDL sobre la película con `File > Import EDL...`, soltando el `.edl` o con click derecho en el clip > `Import EDL Cuts...`: con las flechas Arriba y Abajo saltás de corte a corte, `Shift+U` loopea el plano en el que estás y arriba del visor ves qué plano es.
- **New:** Si al importar una película hay un EDL suyo en la misma carpeta, el Shot Player lo encuentra y te ofrece marcar los cortes con un click.
- **New:** La rueda del mouse acerca y aleja el timeline alrededor del cursor, `Shift` + rueda lo corre de costado y `Shift+Z` lo vuelve a mostrar entero.
- **New:** la primera vez que abrís el Shot Player te cuenta que puede abrir tus EXR, PNG, MOV, MP4, MXF y proyectos con doble clic, y un botón te lleva directo a `File Association` para elegir cuáles.

## v1.001

- **New:** el Shot Player abre y reproduce clips Sony X-OCN de la VENICE (MXF) en tiempo real, hacia adelante y en reversa.
- **New:** Podés asociar los PNG al Shot Player desde File Association: las secuencias numeradas se abren en el Player y las imágenes sueltas en la app que elijas en `Single images open in`, que arranca siendo la que ya los abría.
- **New:** Press Enter (F2 on Windows) to rename the selected clip in the timeline; the name starts selected, so you can also just copy it and press Esc to leave without changes.
- **Improved:** Cada track del timeline muestra su número, que es la tecla que lo muestra u oculta, y un nombre según lo que tiene (comp, aPlate, EditRef o Track), entre como entre el material.
- **Improved:** File Association ordena los tipos de archivo en Image sequences, Movies y Projects, con cada extensión del color de su icono, y los botones de Preferences tienen las esquinas redondeadas.
- **Improved:** The Exposure, Gamma and Saturation sliders keep their tick spacing in smaller windows, showing fewer ticks instead of crowding them together.
- **Improved:** Opening a file no longer keeps the player busy for 12 seconds in the background, so it uses less CPU. (macOS only)
- **Improved:** Playing video uses much less CPU: ProRes, H.264 and HEVC files are now decoded by the Mac's built-in video engine, including 4K ProRes 4444 with alpha and 4:2:2 or 4:4:4 camera files. (macOS only)
- **Improved:** Animation and PNG videos (QuickTime) play with less CPU and about half the memory. (macOS only)
- **Improved:** PNG image sequences, 8 and 16-bit, play with about half the CPU. (macOS only)
- **Improved:** DNxHR HQX and 10-bit DNxHD files play with about half the CPU, and 8-bit DNxHD files (36, 145, 220) and DNxHR LB/SQ/HQ with less CPU too. (macOS only)
- **Improved:** DNxHD and DNxHR files, and other videos the Mac's video engine can't decode, play with about half the CPU and less memory. (macOS only)
- **Improved:** Playback no longer stutters when the Mac is short on memory. (macOS only)
- **Improved:** Rotated or mirrored videos, such as phone footage, play with much less CPU and memory and no longer skip frames when playing backwards. (macOS only)
- **Improved:** QuickTime Animation and PNG movies with alpha play with less CPU and memory, and their colors are now exact. (macOS only)
- **Improved:** Clicking a clip in the timeline only selects it and never moves the playhead; click the ruler or an empty part of a track to move it.
- **Improved:** Selecting clips in the timeline now works like everywhere else: Shift+click selects every clip between the selected one and the one you click, Ctrl+click (Cmd+click on Mac) adds or removes one clip, and Ctrl+A (Cmd+A) selects all clips.
- **Fixed:** Associate en `File Association` vuelve a dejar al Shot Player como app predeterminada en Windows 11, sin que Windows pregunte después qué app usar: antes, en muchas PCs, el botón se desmarcaba solo y el tipo de archivo quedaba sin app para abrirlo. (Windows only)
- **Fixed:** Con varios Shot Player abiertos y poca memoria libre, ya no se cierran de golpe: se reparten la memoria y achican la cache cuando hace falta, con un aviso sobre la imagen. (Windows only)
- **Fixed:** Al abrir un comp con Import Shot Review, el plate entra completo y alineado con el comp: antes, si junto a la secuencia había un MOV del plate, a veces cargaba ese MOV con un solo cuadro.
- **Fixed:** Los videos ya no se traban un instante cada tanto al reproducir, sobre todo los DNxHR largos. (macOS only)
- **Fixed:** Large EXR sequences with alpha no longer skip a frame now and then during the first seconds of playback. (macOS only)
- **Fixed:** 4K Sony XAVC-I files (MXF) play smoothly forward and backwards instead of stuttering at a few frames per second, and XAVC Long GOP (MXF) files are decoded by the Mac's video engine too, with a quarter of the CPU and memory. (macOS only)
- **Fixed:** 4K 16-bit PNG sequences with alpha play smoothly instead of dropping frames. (macOS only)
- **Fixed:** 4K PNG videos (QuickTime), 8 and 16-bit, play smoothly forward and backwards instead of stuttering at a few frames per second, with a third to a half of the CPU and no delay when you start playing backwards. (macOS only)
- **Fixed:** 4K H.264 and HEVC videos, including those with keyframes far apart, no longer skip frames when playing forward or backwards or when you change direction during playback. (macOS only)
- **Fixed:** Stepping to some frames of an HEVC video no longer shows the next frame instead. (macOS only)
- **Fixed:** Playing a video backwards between close In and Out marks no longer drops frames each time playback loops back to the Out mark. (macOS only)
- **Fixed:** Videos with a variable frame rate, such as phone footage, show the same image at each frame whether playing forward, backwards or paused, and no longer skip frames when playing backwards. (macOS only)
- **Fixed:** The dropped frames count in the stats window now matches what you see: it no longer reports drops that never happened, also when playing faster than normal with sound, and it counts the moments the image froze. (macOS only)
- **Fixed:** Reversing the playback direction while playing no longer holds the image for a moment. (macOS only)
- **Fixed:** Changing the playback speed while the sound is playing no longer freezes the image for a moment. (macOS only)
- **Fixed:** Playback no longer stutters for a moment about five seconds after opening a file. (macOS only)
- **Fixed:** With several videos in the timeline, turning a track off or on during playback, or looping back to the start in either direction, no longer makes playback stutter while the video underneath catches up. (macOS only)
- **Fixed:** Keyboard shortcuts such as Space and the arrow keys work again when two player windows are open.

## v1.000 (2026-10-16)

- **New:** Shift+click clips in the timeline to select several, then drag them together with Ctrl+drag (Cmd+drag on Mac), or right-click to sequence them one after another or sort their tracks alphabetically.
- **New:** Shift+Left and Shift+Right jump 10 frames back or forward.
- **New:** A new button next to the snapshot icons saves what you see to the snapshot gallery and opens it in LGA FrameRev, so you can annotate it and save it back to the gallery.
- **Improved:** Help tooltips now show only while you hold Ctrl+Alt (Cmd+Option on Mac), instantly, over the button under the mouse; to see them on hover again, change Tooltip display in Preferences > General.
- **Improved:** The timeline range now always fits every clip: moving a clip past the end extends it, and moving it back shrinks it.
- **Fixed:** The table in Relink Missing Media now shows its scrollbar.

## v0.256 (2026-10-04)

- **Improved:** The player now checks for updates every few hours while it stays open, not only at startup. Remind me later waits one day instead of a week, and closing the update window won't ask again until you restart the player.

## v0.255

- **New:** Drag left or right on the image with the left mouse button to scrub through the sequence, like in RV.

## v0.253

- **Improved:** Update now in the update window and OK in the What's new window are highlighted as the main action.

## v0.252

- **New:** The update window now shows what's new before you install, the app shows it once after an update you didn't see, and Help has a What's new link with the full history.
- **Improved:** In the update window, Update now moved to the right, after the other buttons.

## v0.251

- **Fixed:** Opening a video by double-click sizes the window to the video again, and a session closed maximized now reopens truly maximized. (Windows only)

## v0.250

- **Fixed:** Re-associating a file type (EXR, MOV, MP4, MXF, Shot Player projects) no longer removes other apps' associations for it, and uninstalling Shot Player cleans up the entries it leaves behind. (Windows only)
