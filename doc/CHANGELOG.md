CHANGELOG Unknown Horizons
==========================

| Release | Current savegame revision |
|---|---|
| 2014.1 | 74 |
| 2013.3 | 73 |
| 2013.2 | 71 |
| 2013.1 | 70 |
| 2012.1a | 56 |
| 2012.1 | 56 |
| 2011.3 | 43 |
| 2011.2 | 15 |
| 2011.1a | 12 |
| 2011.1 | 12 |
| 2010.1 | 8 |

- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -

2014-12-31: Milestone 2014.1
----------------------------
changelog date: DEC 31

### Gameplay and Balancing

New features
 - #2207 Only expand settlement range for certain buildings
 - #2201 Color overlays (if running with FIFE 0.3.6 or newer)
 - #2129 Armory producing weapons
 - #2286 Button to fill lumberjack range with trees

Modifications and changes
 - #2187 Change random tree distribution file to clump trees together
 - #2217 Fisher ships now removed together with fisherman building
 - 9411220 Add running costs for warehouse, storage tent, lookout
 - e80ea85 Remove bullets from the attack sequence
 - 56ef8f5 A Pastures starting image depends on its rotation (Rao)
 - #1259 Create inital amount trader ship in ratio to world size
 
Fixed bugs and problems
 - #1824 Salt ponds could be created at fresh water lakes


### Media Content

New files and features
 - #630 Clinker pavilion (tier Settlers)
 - #631 Clinker lighthouse (tier Settlers)
 - #1450 Alvearies for producing honeycombs
 - #1448 Winery
 - ddf6129 Restore warehouse ambient sound
 - #2219 Modified "load from ship", "unload from ship" icons
 - #1788 Spice field
 
Brush-ups and modification
 - #2168 Fix "known incorrect sRGB profile" libpng warnings
 - ee375da Pirate ship flag graphics now consistent with wind direction
 - fcb6dea Update graphics tier bakery (tier Citizen)

### User Interface

Additions and new features
 - #2176 Store (and reload) currently selected tab in savegames
 - #2171 Show resource icons in build menu toolips
 - #2185 Ship pre-selected and in hotkeygroup 1 when starting new game
 - #1387 Status icon for inhabitants without main square connection
 - #2153 Confirmation for pressing Del with unit/building selected (Zappaman)
 - beabc8b Add new key actions for zooming: PgUp / PgDn
 - e886e11 Icons for lumberjack area tree building
 - #2245 Add weaponsmith buildmenu icon
 - #2133 Add simple GUI for atlas generation
 - #2138 Add disaster message icons
 
Repositioning and modifications
 - e6d5239 Rotate mainmenu background images instead of randomizing
 - 3fd3c85 "Iron Mine" is now simply called "Mine"
 - #2182 Tutorial task summary now printed in bold
 - #2189 Dynamic hotkeys in tooltips for certain actions
 - #2200 Larger editor brush sizes
 - #2225 Clear default text for player name and game name (RSouthee)
 - 54a1b59 No longer display Renderer setting in our gui (xml-only now)
 - 7d178e7 multiplayer lobby automatically refresh for new games every 5s
 - efa24b0 Fix resource amount padding in production overview tab

Fixed bugs and usability problems
 - #2176 Doctor and Herbary not available in "per type" build menu
 - 88d051d Consistent cityinfo hide delay for all settlements
 - #2218 Empty inventory slots incorrectly stretch their icon
 - d064f37 Only show "warehouse not tearable" message for own warehouses
 - #2136 No more color confusion between SP and MP menu (pinkfloyda)
 - #1966 Transparent nature buildings around destroy tool (Zappaman)
 - #2267 Restore layout of production line tabs with multiple resources (dulrich)
 - #1790 Scenario messages being displayed only after Logbook is hidden
 - #2210 Wrong status icons at startup (dulrich)


### Codebase

New functionalities
 - #2173 Manpage generation with custom optparse formatter
 - #2229 Add the ability to set a default build menu style (Zappaman)
 - 5038c59 Cache XML read from the harddrive
 
Modified structures
 - #2175 Tabwidget code refactoring
 - #2174 Save/load helpers for game tests and gui tests
 - #2184 Introduce content/packages/ for files related to packaging
 - #2181 More readable filenames for auto- and quicksaves
 - 3847de7 Make LAYERS.WATER static (zoom performance)
 - 2811241 Extract atlas loading into thread
 - 42abaf1 & #2130 Use unicode to log errors
 - 37e5a73 Allow generic unit command for network usage

Fixed crashes and inconsistencies
 - #2177 Several fixes for OS X app container
 - #2193 Survive invalid minimap preview data
 - #2197 Settings now upgrade properly again
 - #2221 time.strftime crash on loading savegame with non-utf8 locale
 - #2231 Prevent a crash when losing network connection
 - #2244 Some Fife OpenGL settings were not applied
 - #2287 Crash when clicking on ship in savegame
 - #2289 Multiple PEP8 changes (MarkusHackspacher)
 - #2113 Fix trade route handling in multiplayer games

 
### User-Contributed Content

Translations
 - New: Traditional Chinese
 - New: Afrikaans

Campaigns, scenarios and maps
 - Update tutorial text (paul59)

New team members with this release, Annotations
 - Push access was granted to:
     janexx
 - We accepted pull requests or patches by:
     phaidon, RSouthee, Zappaman, pinkfloyda, myrdd, Rao, MarkusHackspacher, paul59
 - Translators that joined our teams and contributed several strings:
   Please refer to the credits!

- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -

2013-10-04: Milestone 2013.3
----------------------------
changelog date: OCT 02

### Gameplay and Balancing

New features
 - #2116: Black Death disaster
 - #2119: inventory overlays (if running with FIFE 0.3.6 or newer)

Modifications and changes
 - #2151: MP save/load disabled for this release due to bugs
 - 04498fa: only enable update checker for platforms without proper
   package management (Darwin and Windows)

Fixed bugs and problems
 - 9d4a7e1: crash when clicking on messagewidget messages in scenarios
 - #2039: introduce memory leak to fix `RuntimeError: _[NotFound]_ ,
   Something was searched, but not found :: action move_as_[corrupted]`
 - #2078: crash when joining password-protected multiplayer game
 - #2143: crash on update check timeout when master server unavailable
 - #2164: Allow scenario savegames to load again


### Media Content

New files and features
 - #1791: indication that a scenario task has been completed

Brush-ups and modification
 - 

### User Interface

Additions and new features
 - d413693: improved loading screen messages about current stage
 - #2070: interface to change hotkeys in settings
 - #2094: return key confirms singleplayer, multiplayer and editor menu
 - 8d0d248: `PAUSE` as secondary key for pausing game (primary: `P`)
 - #2098: display gameplay tips in help screen
 - #1630: option to disable FPS limiter

Repositioning and modifications
 - #1310: right clicks in trade route resource selection are now
   special-cased to abort selection (not empty slot) sometimes
 - 420e17d: `LOGBOOK_DEFAULT_DELAY` reduced to 1-4 seconds (was: 4-7)
 - 800cc2b: use ellipses (`…`) instead of `...`
 - #2106: many changes to settings dialog

Fixed bugs and usability problems
 - #2081: explanatory labels for map editor
 - #1789: show message text next to corresponding icon
 - #1587: show correct logbook section when scenario goal is reached
 - #1577: messages of accomplished scenario tasks disappear
 - #2111: closing logbook creates notification for finished objectives
 - #1975: toggle "ready" text and button in MP lobby depending on state
 - #2161: move menu buttons for consistent navigation and layout


### Codebase

New functionalities
 - #2077: lazy translation (`speaklater` library)
 - 3195744: script to update existing translations against new template
 - #2100: scenario condition `game_started`
 - #2160: handle API changes expected towards FIFE 0.4

Modified structures
 - #2106: huge rewrite of settings handling
 - #2053: default hashbang now is `/usr/bin/env python2`
 - #2058: allow running with FIFE newer than 0.3.4
 - 0a1d6db: migrate script to translate a scenario to python
 - 58a192d: correct location comment for xml-extracted translations
 - #2088: copyright headers now `2008-2013` instead of just `2013`
 - 771b65e: `SimpleMessageBus` allows same callback only once per message
 - #2090: 'metadata' container for scenarios, rewrite scenario menu
 - 47c50a2: remove reference to main gui in session
 - 125ed7a: stop inheriting from ApplicationBase
 - #2104: minify i18n module, move pychan-related code to `horizons/gui`
 - #2125: unify defaultdict arguments
 - c08ba01: FIFE version check switched from svn to major, minor, patch
 - #1945: move atlas generation to `horizons.engine`
 - #2149: rename `server.py` to `run_server.py` to disambiguate

Fixed crashes and inconsistencies
 - 3c363f4: handle unknown actions in hotkey settings
 - 35d73e7: pressing S on loading screen before gui initialized crashed
 - #2121: detect and skip empty scenario files
 - b36f5ca: work around an error occurring when ColorID setting was 0
 - 971553d: rare crash when denying upgrades to inhabitants
 - #2162: Forget about failed minimap-generating subprocesses


### User-Contributed Content

Translations
 - Now hosted on http://hosted.weblate.org/projects/uh/
 - New subproject containing files for eventual speech translation
 - 3c32538: Replace some `python-format` with `python-brace-format`

Campaigns, scenarios and maps
 - 

New team members with this release, Annotations
 - Push access was granted to:
 - We accepted pull requests or patches by: alluk, Daenor
 - Translators that joined our teams and contributed several strings:
   Please refer to the credits!

- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -

2013-04-06: Milestone 2013.2
----------------------------
changelog date: APR 06

### Gameplay and Balancing

Modifications and changes
 - reduce boards upgrade cost of all residential buildings by 1
 - rename 'increment' to 'tier'

Fixed bugs and problems
 - boatbuilder eating the player's money - #2046
 - re-enable almost all ambient sounds
 - residences being affected by disasters shouldn't upgrade - #1835
 - undefined boat builder behavior when pausing construction and ordering new ship - #1830
 - crash on special unloading and loading combinations - #1999


### Media Content

New files and features
 - warehouse graphics for tier 3 (Daniel)
 - Use player-colored settlement icon in cityinfo and account tab
 - music track: Ireland's Coast by Matthew Pablo
 - music track: Peer Gynt Suite No. 1, Op. 46 - I. Morning


### User Interface

Additions and new features
 - allow multiselect combinations of units and buildings
 - start savegames with doubleclick - #2036 (ThePawnBreak)
 - support for different buy and sell prices (ThePawnBreak)
 - information about price in tooltip in Select Resources widget (ThePawnBreak)
 - necessary resources tooltip to build menu - #1886 (ThePawnBreak)

Repositioning and modifications
 - update distillery and charcoal burning build menu icons
 - Buildingtool: tweak color highlights

Fixed bugs and usability problems
 - multiselect tab crashes after hiding it when pressing delete
 - clicking on multiplayer menu crashes when there's no internet connection
 - certain ToggleImageButtons segfault on hover - #2000
 - cityinfo widget position with large resource overview bar - #1866
 - crate icon in overview of resource deposits - #2001
 - Remove same version only checkbox in multiplayer menu - #2068


### Codebase

New functionalities
 - quicksave and autosave for editor - #1935 (ThePawnBreak)
 - progressbar on loading screen
 - font change on runtime - #1740
 - script to create a linux tarball
 - TilingProgressBar that tiles its fill image instead of stretching

Modified structures
 - multiplayer sever only returns games running the same protocol version
 - remove unused and outdated install script
 - make the AI try to react to disaster and mine depletion events only when they are about that player
 - leave the MP game when the game lobby is cancelled

Fixed crashes and inconsistencies
 - hitting Esc while loading screen is active crashes - #2018
 - multiplayer backward compatibility for 2012.1
 - Remove double extensions (.sqlite.sqlite) from savegames - #2065

New team members with this release, Annotations
 - Push access was granted to: ThePawnBreak
 - Add gryffus to AUTHORS, packaging for Fedora and openSUSE Linux distribution.
 - Translators that joined our teams and contributed several strings:
   Please refer to the credits!

- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -

2013-01-27: Milestone 2013.1
----------------------------
changelog date: JAN 27

### Gameplay and Balancing

New features
 - AI players learned to handle diplomacy and war
 - new buildings: alvearies, barracks, blender, cocoa field, doctor,
   herbary, lookout, pastry shop, spice field, vineyard, vintner
 - build preview jumps to valid build locations nearby
 - production building storage indicators when finishing production

Modifications and changes
 - collectors pick up resources produced while walking over - #929
 - collectors can retrieve multiple resources at the same time - #994
 - fire station: 4 bricks (was: 5), tavern: 4 bricks (was: 2)
 - trees take 120s to grow (was: 60) and cost 50 gold coins (was: 10)
 - producing boards requires 2 trees (was: 1)
 - charcoal production consumes 3 boards (was: 5)
 - increase storage size for coal in the charcoalburning to 4 (was: 2)
 - Messages now only displayed once in scenarios - #1897
 - don't allow empty names for ships and settlements
 - allow frigates to trade - #1989
 - require buildings other than warehouses to be entirely within settlements - #1970, #969

Fixed bugs and problems
 - fixed wrong graphics of tree growth sequence - #924
 - burnt down residential buildings replaced by ruin
 - save freetrader, pirate and disaster settings - #1372


### Media Content

New files and features
 - new tileset graphics (Daniel)
 - docs: contribution guidelines
 - font: GNU Unifont as general font fallback
 - sound: error sound, refresh sound, click sound (Kinshuk)
 - building: three citizen houses, citizen street (Viktoria)
 - building: pioneer, settler, citizen main square (Viktoria)
 - building: barracks, brewery, herbary (Daniel)
 - building: doctor (mrkramps)
 - unit: fisherman (Daniel)
 - music: track "Battle" (Thomas Davey)

Brush-ups and modifications
 - resource icons are now 32px everywhere
 - buildings retain their rotation when upgraded
 - remove alpha palette from fish images - #1906


### User Interface

Additions and new features
 - Balance display in top left corner (click to expand) - #1671
 - loading screen displays gameplay tips and quotes (toggle in settings)
 - new cursor above TextFields when keyboard input is possible - #674
 - Esc triggers the cancel action, Enter the ok action in all dialogs
 - kick players in multiplayer lobby, 'ready' flag to start game
 - password protection for multiplayer games
 - menu background image can be toggled and persists
 - mouse wheel zoom behavior can be changed in settings
 - list to select available scenario translations, shows completeness
 - error sounds for invalid and impossible actions
 - click sound for all gui actions
 - second build menu layout (toggle with icon)
 - new ingame map editor, replaces the old external one
 - new widget to show FPS via F10

Repositioning and modifications
 - BuildRelated tabs now use one line per tier
 - cleaned up and polished production overview, inventory tabs, boat
   builder, main square, inhabitant overviews, trade route config
 - mouse wheel no longer changes ListBox selection, only scrolls view
 - highlight fish deposits in range of fishers, improve fish highlight
 - dynamic cityinfo placement, depends on resource overview bar size
 - popups now modal by default
 - reworked layout of Game-Settings page - #1751
 - use 'abcd' image for roads as buildpreview if it exists
 - restyle city info

Fixed bugs and usability problems
 - only display status icons when and where they make sense
 - multiplayer: check required building costs early - #1486
 - do not show fisher boats on minimap
 - used action sets are stored in savegame
 - clicks on scenario messages open corresponding logbook page
 - warehouse selection unintuitive - #1246
 - select most recent savegame in "Load game" dialog
 - make the coordinates tooltip show integer coordinates again
 - save max tier notification per player
 - update building preview on player or settlementinventory change - #1680


### Codebase

New functionalities
 - icon_path and delayed updates are now available in TabInterface
 - setup: creates `content/gitversion.txt` containing detected git HEAD
 - build menu layouts can be defined via yaml
 - 'fife' logger, activate by `--debug-module='fife'` or `-d`
 - scenario actions:
   `highlight_position`, `change_increment`, `alter_inventory`
 - scenario tests
 - store hotkey key values in settings file - #1302
 - add enet.so library for x64 Mac users with system python 2.7
 - new atlases generator, enable/disable via settings.xml or commandline
 - add the `--no-freeze-protection` flag to disable freeze protection
 - show a warning of unsupported fife revision
 - silently upgrade savegames our savegame upgrader can upgrade
 - add the `--edit-game-map` option to edit the maps of saved games
 - GCI Scroll Settings - #720

Modified structures
 - own implementation of yaml cache, replacing shelve
 - less verbose api for horizons.messaging
 - soft constants instead of hardcoded numerical ids in yaml files
 - moved some more properties to yaml object files
 - `--nature-seed` flag is gone, `--sp-seed` provides its functionality
 - rewrote mp client/server methods, support older client protocols
 - globals in horizons.main now live in horizons.globals
 - remove support for preview action sets, allow weighting action sets
 - use yyyy-mm-dd.nn format for profiling data files.
 - rename `--load-map` to `--load-game`
 - remove the entire campaign system

Fixed crashes and inconsistencies
 - use unicode everywhere, only convert it when talking to fife
 - storages provide `itercontents()` and `iterslots()`
   instead of `__iter__`
 - invalid LC_TIME, LANG, LOCALE environment variables no longer crash
 - add workaround for FIFE's inconsistent instance rotation round
 - Fix animal location saving


### User-Contributed Content

Translations
 - new translation project: multiplayer error messages
 - new translations: ml, uk
 - new terminology translations: uk
 - new tutorial translations: ml, uk
 - new translations of 'The Unknown': de, es, fr, nl, pt_BR

Campaigns, scenarios and maps

New team members with this release, Annotations
 - Push access was granted to: mesutcank, Kiryx,
 - We accepted pull requests or patches by:
   Foaly, Srijan Mishra, Vivek Sagar, MasterofJOKers, Magnus Knutas,
   desophos,
 - Translators that joined our teams and contributed several strings:
   Please refer to the credits!

- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -

2012-04-22: Milestone 2012.1
----------------------------
changelog date: APR 22; rev: 589a1f461b749b1d05bd29ae7e73dd19ce52677f

### Gameplay and Balancing

New features
 - screenshots of savegames
 - highlight buildings in range in construction preview
 - map preview, using a subprocess
 - disasters: fire as proof of concept, fire station as remedy of choice
 - allow generating different random maps and using own random seeds
 - status icon system for buildings
 - major overhaul of buy/sell interface
 - major overhaul of resource overview bar, custom bars per settlement
 - many new hotkeys (see section User Interface)
 - statistics widgets: player scores, settlement/ship overview, chat history
 - Unknown Horizons automatically checks for updates on startup
 - support for CJKV translations
 - save/load in multiplayer games

Modifications and changes
 - AI founds more settlements
 - lower running costs for several buildings when paused:
   * charcoal burning, distillery, farm, tobacconist, weaver: 0 (was: 5)
   * salt ponds: 0 (was: 10)
   * doctor: 5 (was: 15)
 - maximum game speed now: 20x
 - multiplayer mode: game names
 - boat builder now displays queue and allows modifications
 - "Branch Office" renamed to "Warehouse", "Tent Ruin" to "Ruined Tent"
 - only allow fires from the 2nd increment onward
 - signal fire range now: 13 (was: 10)
 - make fisher invincible
 - trader: Sell and buy for same price, increase max amount
 - round displayed resource values
 - make the AI work better on level 4
 - make trade make smaller offers in case settlements don't accept big ones
 - don't pause game on routeconfig (#1692)
 - make mountains unclonable (#1703)

Fixed bugs and problems
 - main square and ruined tent now walkable, i.e. behave like a road
 - ships only load as many tons of a res as specified in the route at max
 - fix count problem in warehouse buy/sell tab
 - assign appropriate level to settler on build (#1561)
 - crash on hovering the resource overview bar (#1564)
 - crash when trying to drag a line of buildings on the ocean (#1574)
 - crash when pressing "j" while a building is selected


### Media Content

New files and features
 - building: new fish (lmg)
 - building: fire station
 - building: single tile roads
 - building: all rotations for the birch tree
 - building: windmill
 - building: bakery
 - animated status icons: full inventory, decommissioned, mine cart, book
 - animated status icons: question mark, exclamation mark, building on fire
 - sound: invalid actions / error
 - sound: build sound (Novatlan)
 - sound: flipping page
 - icon: capacity utilization (also used for other stats)
 - icon: different happiness stage smileys
 - icon: pipette cursor
 - icon: rename (20 and 50px)
 - icon: ship on minimap
 - icon: animated cogs for active production lines
 - icon: medium and large popup background images
 - icon: three new mainmenu background images
 - icon: messagewidget background images
 - icon: new icon for tobaccos (#692)
 - icon: Leather and tannery icons (#692)
 - unit: animated pirate ship
 - font: UMing for CJKV

Brush-ups and modifications
 - building: new renders of charcoal burning
 - building: new renders of distillery
 - building: improve increment 3 house
 - icon: save/load in main / pause menu
 - icon: inhabitant amount
 - icon: minimap background image
 - fish animations run at different speeds
 - overview bar resource selection menu default config button style
 - 300px UH logo
 - Make farm use small cogs in production animation (#1474)
 - 24px flour icon (#1594)
 - new images of the mine and mountains (#906)
 - update and reposition FIFE logo


### User Interface

Additions and new features
 - tooltips for status icons
 - prices are now displayed in the hint for selling/buying resources
 - minimap in ship route config dialog, click on BO to add it to the route
 - sending ships via click on minimap, highlight selected ships in minimap
 - captain's log entries can now contain images and multiple entries per page
 - pipette tool to clone existing buildings (O)
 - save and show trade history
 - support for dynamic hotkey configuration
 - hotkey A to display owner color on tiles
 - hotkey J jumps to selected units
 - hotkey K toggles healthbars
 - hotkey R to enter road building mode
 - enter key confirms a popup
 - delete key removes units and buildings
 - zoom to mouse position as new center
 - remove resources in buy, sell, load, unload slots on right click
 - setting for mouse sensitivity
 - setting to enable logging
 - setting to disable auto-unloading goods on founding settlements
 - highlight position of messagewidget events on minimap
 - show unit route on minimap when player owns selected unit
 - build multiple tents by holding the mouse (same as trees)
 - dynamic build menu (highlight buildings currently buildable)
 - show building costs when hovering build menu buttons
 - highlight related buildings in build preview mode
 - enhanced player name and color selection
 - re-enabled map panning with middle mouse button
 - display random background image in mainmenu
 - load and display messagewidget items in logbook game message widget
 - setting for number of frames per second
 - add minimap icon for pirate and neutral ships
 - colored flags for minimap ship icons
 - notify the player when his buildings catch fire

Repositioning and modifications
 - improved random name selection algorithm (prefer unused names)
 - improved diplomacy UI and messages
 - sliders for map creation always start in center position
 - ship status now clickable in ship list
 - show warehouse locations on minimap
 - combine widgets minimap and menu_panel to new widget 'minimap'
 - simplified ship and main square tabs
 - tooltip explanations of some settings
 - minimap and tabwidget positioning changed: prevent unintentional scrolling
 - RouteConfig: Move activity icon into focus of attention area
 - zooming depends on cursor location
 - brighter and hopefully less obtrusive range highlight colors
 - multiselection improvements
 - improved resource configuration restore button
 - end session when the game is closed
 - individual shipicons on the minimap
 - Use abcd shape as preview image for trail, gravel path
 - only show building range when the building is buildable
 - display building costs even if it's not buildable at the current position

Fixed bugs and usability problems
 - reduce tooltip flickering
 - camera view rotation directions were incorrectly named
 - show message when autosaving
 - faster first access to pause menu
 - mousetool destruction between sessions
 - sound got cut off on scroll (#1277)
 - sort players in player scores overview according to total score
 - add summary to settlement list
 - rotate natural resources randomly
 - add savegame date and time to filenames
 - main widgets could be displayed twice, resulting in an infinite pause loop
 - build roads clockwise or counterclockwise based on user input
 - display hint when a field is fully grown, but has no farm access
 - consider keyboard scrolling when determining active settlement
 - also show radius of signal fire on sea tiles
 - stay in warehouse build mode when trying to build at invalid location
 - delay cityinfo hide after hovering own settlements, renaming improvements
 - allow to rename ships/settlement in statistics widget
 - notification threshold depending on event distance wrt. time and space
 - lots of is_focusable fixes (buttons previously caught keyboard events)
 - keep gold amount widget stable (don't blink) in resource bar (#1560)
 - allow logbook entries with multiple pages and always show first new entry
 - fix problem with minimized minimap ship icons
 - stop scrolling when the mouse leaves the window
 - stop windmill animation if decommissioned (#1625)
 - distinguish idle and idle_full of our mill
 - make esc close the chat dialog
 - don't show decommissioned status of buildings that shouldn't have them
 - do not run update checker with gui tests or cmd line start parameters


### Codebase

New functionalities
 - Components!
 - MessageBus and Message system
 - gui logger (store all input actions) to help creating gui tests
 - pre-commit hook for developers
 - interactive iPython shell: allows executing any available Command
 - support for gui tests and many gui tests
 - tests can make use of savegames
 - map saver and loader plugin for editor
 - script to pull and compile .po files from translation repository
   (development/copy_pofiles)
 - change pychan widgets on runtime for tooltips to use `helptext=`
   attribute
 - `comment=` widget attribute as context help for translators
 - save random map settings to settings.xml file
 - save maps (shift + F12)
 - status icons above buildings and units, status icon exclusions
 - minimap highlights
 - cmd line option `--game-speed`
 - use fife.Point.set where reasonable (performance)
 - lazy loading for tabs
 - dynamically update data of older savegames to current format
 - locale-aware fontdef loading (LinLibertine vs. UMing)
 - support starting 2-player mp game via command line
 - coupling between selectability and tabs
 - session property for all components
 - stop multiplayer game when detecting desync, print hash differences
 - modular messagewidget (dynamic height depending on message)
 - use YamlCache for object files to speed up loading
 - several robustness improvements to YamlCache
 - make catching gcn::exceptions more robust
 - add tests for buildingtool highlights, hunter and settler save/load
 - add new enet library-files
 - add mac build support

Modified structures
 - adapt all widgets to new pychan keyword API
 - removed all custom Tooltip* widgets
 - speed up build mode by 40%, and by 6000% for buildings with related
   buildings
 - allow human-readable resource ids in object files, like RES.FOOD
 - refactored i18n methods to replace widget content
 - improved loading speed for production lines, PathNodes,
   AbstractPather, ComponentHolder and GlobalLimitStorage
 - minimap no longer uses GenericRenderer and supports more than one
   minimap instance
 - road pathfinder now prefers straight lines
 - default ai player amount is 0 for games started from cmd line
 - save tile ownership instead of autogenerating it on load
 - speed improvements to loading/saving huge settlements (scheduler)
 - inventory tab uses ExtScheduler instead of Scheduler
 - refactored management of all mousetools
 - rename ConcretObject to ConcreteObject
 - building and unit outline parameters (threshold, width) now
   configurable
 - now using python's `'{foo}'.format(foo=bar)` for all i18n strings
 - use python string formatting instead of string.Template
 - store savegame template as sql statements instead of binary sqlite
   file
 - lazy loading of action sets
 - level-depending building names (lumberjack tent -> lumberjack hut)
 - exclude certain status icons from certain buildings
 - save language code instead of language name
 - settings and logbook now use a PickBeltWidget
 - removed several tables from our database. Data now in yaml objects.
 - registry pattern to keep track of scenario actions/conditions
 - large amount of fixes and workarounds for styling widgets
 - removed log.yaml and useless Bridge class
 - modularize all the buildingtool functions
 - explicit imports in horizons.i18n
 - move language switch logic and gettext setup to horizons.i18n

Fixed crashes and inconsistencies
 - reduced memory leaks when ending a session
 - more than 40 crashes related to merging the branch "component"
 - crash when clicking on savegames in save dialog (#1223)
 - uninterrupted building setting now also affects destruction tool
 - crash when player name contained unreasonable characters
 - sand tiles are buildable again
 - crash when removing main square
 - trader now respect settlement needs when selling
   (buying 1 unit was impossible)
 - routeconfig crash
 - faulty parameter name caused endless loops when FIFE was not found
 - crash with inaccessible entries in guitranslations
 - rounding issue caused problems with minimap
 - handle random crashes that are defined behavior for python shelves
 - use os-independent paths in the savegame manager
 - crash when trying to overwrite a read-only file on windows
 - some bugs in our core scheduler and timer code


### User-Contributed Content

Translations
 - new translations: ja, ro, hr
 - new terminology translations: ja, ro
 - new tutorial translations: bg, et, hu, ja, ro
 - updates to translations: bg, ca, cs, de, es, et, fi, fr, hu, it, lt, nb,
                            nl, pl, pt, pt_BR, ru, sl, sv
 - updates to tutorial translations: cs, de, fi, fr, pl, ru

Campaigns, scenarios and maps
 - removed old maps and islands (incompatibility with new tileset structure)
 - new island: bay_and_lake
 - new maps: development, mp-dev, singularity40, triple, test-map-tiny
 - new maps: quattro, Full House (3 pl), Rouver (4-6 pl), FightForRes
 - new scenario: The Unknown by Kikody
 - new scenario: deathmatch
 - included images in tutorial scenarios

Media Content

New team members with this release, Annotations
 - Push access was granted to:
 - We accepted pull requests or patches by:
 - Translators that joined our teams and contributed several strings:
   Please refer to the credits!


- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -

2011-11-11: Milestone 2011.3
----------------------------
changelog date: NOV 11; rev: 52f9d95664860098e1a53f5995b3e7a84b9ce32c

### Gameplay and Balancing

New features
 - trade routes can wait for load and unload
 - support for international trade routes: player<->player trade
 - new in-game pause menu, replaces pause popup and in-game menu
 - hotkey `T` toggles translucency of trees and mountains
 - player score widget, accessed through F2
 - player settlement overview, accessed through F3
 - player ship list, accessed through F4
 - allow/deny inhabitant upgrades
 - show hint when user tries to build something without a settlement
 - option to build uninterrupted (was: need to hold SHIFT)

Modifications and changes
 - unload all resources in ship inventory when a new settlement gets founded
 - allow lower resolutions until 800x600
 - rename market place to main square
 - modified ALL resource values, refer to `development/print_db_data.py res`
   for the new values. Drastically lowered the price of most resources.
 - settler consumption formula now properly considers number of inhabitants
 - settler tax and happiness formula
 - increase base taxes paid by one settler level. Now 3/6/10 (was: 2/3/6)
 - game speed array now is [0.5x 1x 2x 3x 4x 6x 8x 11x]
 - 'raw' resources now have reasonable names (sugar cane, tobacco plants).
   Also renamed raw iron and raw clay to iron and clay deposit, respectively.
 - better distribution of resource deposits
 - player starts with 12 cannons
 - fisher boats cannot be built as of now
 - boat builder allows construction of huker and frigate
 - open ship inventory tab after trade became impossible (ship left BO range)
 - free trader and fisher boats are invincible
 - boat builder and branch office build restrictions: need deep sea water now

Fixed bugs and problems
 - mutable default arguments caused resource deposits to be empty
 - check full area of branch office for other settlements before building
 - loading caused decommissioned buildings to have active production costs


### Media Content

New files and features
 - building: gravel path
 - building: wooden storage hut
 - icon: diplomacy in minimap panel
 - icon: trade route slot modes (load ship, unload ship)
 - icon: trade route access buttons
 - icon: combat stances aggressive, hold ground, none, flee
 - icon: allow/deny inhabitant upgrade
 - icon: several build menu and resource icons
 - voice: french map_creation by seblabel
 - colors: purple, orange, teal, lemon, bordeaux, gray

Brush-ups and modifications
 - icon: all minimap panel icons
 - icon: all player emblems (also added new ones)
 - font: update Linux Libertine to version 5
 - image: more saturation for main menu background


### User Interface

Additions and new features
 - random map parameters: island size (max, mean, sd), map size, water ratio
 - map parameters in UI: AI players, resource density, free trader and pirate
 - save random map parameters to settings file
 - display error message when yaml can't be found
 - build menu now updates when inhabitants upgrade
 - buoys now also displayed for user interactions like trade routes
 - show hint when user tries to build something without a settlement
 - recommended players per map displayed in map selection widget
 - notification messages about why trade actions were invalid

Repositioning and modifications
 - use unicode strings for all ship names
 - use templates for different boxes in singleplayer menu
 - removed need for adjust_black_background
 - slim minimap images, icon positioning in minimap panel
 - remove the main square overview tab
 - reposition city_info on low resolutions to not overlap HUD
 - `=` key now also increases game speed (was: `+` only)
 - pausing the game disables all game interactions
 - city_info now displays player emblem

Fixed bugs and usability problems
 - boxes in settings expanded for some languages, buttons were unreachable
 - in-game ui appeared around the main menu under certain conditions
 - trying to save in multiplayer no longer causes a crash
 - recognize the system default language on windows
 - display warning if pyenet is not found and disable multiplayer (was: crash)
 - cancelling a build action issued through 'Build related' opened build menu
 - removed problems with highlight cache (TearingTool cleanup)
 - display needed resources if hovering 'Found settlement' in ship overview
 - disable game speed buttons when min / max is reached or the game is paused
 - disable speed buttons in MP session
 - clearly indicate that increment 3 is the current maximum
 - remove building-specific Destroy Building button. Use Destroy tool (X key)
 - instantly redraw building range (was: delayed for at least 0.1 seconds)
 - immediately update cam after click
 - frigate overview tab fixed


### Codebase

New functionalities
 - support explicit paths to files for `--start-map` `--load-map`
   `--start-scenario` and `--start-campaign`
 - save and load the rng state
 - scenario action for spawning ships
 - dev script to generate a gfx overview website
 - unified statistics widget
 - 'noi18n' name for widgets that are not planned to be translated
 - speech implementation
 - gzip logfile compression
 - dev cmdline option `--no-preload` to never start preloading
 - tool to generate statistic for MP server using rrdtool

Modified structures
 - deselect instances before removal
 - use `%APPDATA%\unknown-horizons` as user dir on windows
 - Settlement now is a StorageHolder for consistency and simplicity
 - huge improvements to pathfinding speed
 - use plain text sql statements instead of binary sqlite databases
 - removed some outdated sql tables
 - obsolete and misleading FarmerCollector replaced by BuildingCollector
 - modified size of rect created by Rect.init_from_topleft_and_size
 - max player value also limits amount of AI players
 - captain's log now also uses StatsWidget
 - rename build menu icons to use building ID (was: ambiguous building name)
 - temporarily remove settler.sql
 - game data on windows now stored in My Games
 - multiplayer code refactoring. Includes command whitelisting for safety
 - DistUtilsExtra no longer is dependency for building i18n files
 - removed adjust_widget_black_background

Fixed crashes and inconsistencies
 - most tests crashed on windows (open file handle)
 - scheduler removes callbacks of current tick as well now
 - catch exceptions that happened during 'reset settings to default'
   this lead to a crash right at start for players with older settings.xml
 - missing import which caused a crash when starting multiplayer
 - several crashes related to removing units and buildings
 - upgrading python to a version not supporting bsddb anymore caused crash
 - loading games could fail on mac due to `.DS_Store` files in `content/`
 - two segfaults related to quitting the game
 - collectors now teleport home if they cannot find a way home
 - crashes related to ship removal and AttackCommand
 - animal pathfinding crashes: blocked path while being built on
 - problem with utf-8 in filenames on the windows console
 - no yaml cache if utf8 characters in windows username (bsddb bug in python)
 - crash related to FIFE console evaluations overwriting gettext `_`
 - crash on compaign startup
 - UnitProduction endless loop fixed
 - Ships sailing on land
 - StorageCollector endless loop fixed
 - resource deposits stay selected after being removed
 - selection not removed after tearing
 - unit health bar is rendered correctly


### User-Contributed Content

Translations
 - new translations: sv
 - new terminology translations: sv
 - new tutorial translations: cs, es, pl, pt_BR, sv
 - updates to translations: bg, ca, cs, de, es, et, fi, fr, hu, it,
   lt, nb, nl, pl, pt, pt_BR, ru, sl
 - updates to tutorial translations: de, fi, fr, it, nl, pt, ru

Campaigns and scenarios
 - new scenario 'war_tutorial' by mihaibivol

Media Content

New team members with this release, Annotations
 - Push access was granted to:
   wentam
 - We accepted pull requests or patches by:
   hoffi, abeaumont, orakeldel, mtfk
 - Translators that joined our teams and contributed several strings:
   Please refer to the credits!


- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -

2011-07-01: Milestone 2011.2
----------------------------
changelog date: JUL 01; rev: 5bfb7f58f2c8fd8cb3e16185ff5b510b752fc4ba

### Gameplay and Balancing

New features
 - option to disable edge scrolling with mouse
 - basic customizable trade routes for ships
 - pirates with home position sail around and chase player ship
 - improvements to random map generation time
 - improvements to savegame loading time
 - scenario chooser interface after winning a scenario
 - improvements to pathfinding speed on sea tiles
 - randomized playlist of background music
 - first version of production overview widget
 - display hint to tell players that roads can be dragged when detecting that
   they build them one-by-one

Modifications and changes
 - tavern building costs: 250 coins, 4 boards, 2 bricks (was: 0, 0, 0)
 - sugar cane field building costs: 150 gold coins (was: 0)
 - storage tent building costs: 350 coins (was 750), 4 boards (was: 10)
 - storage tent additional capacity per slot: 10t (was: 30)
 - storage tent radius: 17 (was: 24). Reduces the covered area by 50%.
 - use pirate ship names for pirates (was: player ship names)
 - show empty logbook (was: silently not show)
 - more useful error messages: description, advice, technical details
   (was: description, technical details)
 - update inventory once a second (was: on every settlement change)
 - apply changes to autosave interval at runtime (was: only after restart)
 - inhabitant taxes can now be set in 10 steps of 0.1 (was: 3, 0.5)
 - only display scenarios in selected language and English by default
   (was: display all scenarios)
 - tearing tool sticks if shift key is pressed, same as building tool
 - ships only have a limited amount of slots now (was: unlimited - GUI: four).
   The overall storage limit can be distributed without further restrictions.
 - ships of other players now have overview tabs (was: None)
 - tabs of enemy buildings and units tell the player name of their owner
 - clay found in deposits now between 750 and 1250 (was: 375, 625)
 - spawn more animals at game start, probability 10% per tile (was: 2.5%)
 - search more efficiently for targets when moving ship to unreachable coords
 - improvements to wild animal health balancing

Fixed bugs and problems
 - show player's gold immediately after load
 - handling of multiple dialogs that pause the game (new pause stack)
 - reset of tile walkability after buildings have been removed
 - Made trader a bit faster when it can't find a path to a branch office
 - route entry slot was reset when adding new resource
 - fishers no longer get stuck as easily
 - paused game allowed to change game speed
 - only allow grouping of units owned by the player
 - remove fisher outline when deselected
 - ask for confirmation before restoring default settings in the settings menu
 - WildAnimal did not reproduce


### Media Content

New files and features
 - building: sugarcane field
 - building: tavern
 - building: half-timbered house
 - icon: up and down arrows, small rect-shaped delete button
 - icon: svg application icon without text for use in small icons
 - icon: grayscale version of speed_* minimap panel buttons
 - icon: small 16px versions of more resources
 - unit: lumberjack
 - simple script that helps adding names to the database

Brush-ups and modifications
 - tooltip graphics
 - tab background images
 - pasture animated with more frames
 - save icon in game menu


### User Interface

Additions and new features
 - ship name label and dynamic spacing in trade / exchange widget
 - settings for multiplayer connection (network)
 - display settlement name as heading in some buildings
 - added tooltips to several buttons and labels
 - display tax rate as label
 - highlight background of currently selected tab
 - first version of tab 'build related fields' for e.g. farm and lumberjack

Repositioning and modifications
 - dynamic positioning on most headlines. Causes intentional glitch
 - made random maps prettier, coastline is now properly drawn
 - default style border size now 0 (was 2)
 - button placement in settings
 - display correct residential names in inhabitant overview tab (was: 'Tent')
 - added scrollareas to credits

Fixed bugs and usability problems
 - duplicate string name in help.xml that caused wrong translation
 - spacing issues with headline of build preview tab when rotating the preview
 - 'Widget containment fumble' warning in buyselltab selection widget
 - properly translate tooltips in build menu
 - buy/sell tab no longer displayed at storages, now only available at branch
   office and main square


### Codebase

New functionalities
 - test infrastructure
 - large amount of tests
 - string preview tool for translators: start with `--string-previewer`
 - starting random maps with specific seeds from the command line
 - support for UPnP + NAT-PMP (using miniupnpc, libnatpmp and their python
   modules). For now this will only work on unix because there is no
   socket.fromfd on windows for python2.
 - added compatibility layer for pyenet build with pyrex vs cpython
 - storage capacity can now be set for each storage building
 - StepSlider that snaps to values
 - auto-style each widget named 'name' or 'headline*' as headline style
 - using a cache for ImageFillStatusButton in inventories
 - filter destination points in pathfinding
 - made Callback class hashable for usage in dictionaries
 - cache yaml files unless altered. Faster scenario selection in SP menu.
 - testing gettext plural form support
 - execute_many available in DbReader
 - passing seed to RNG for all session types, use constant seed by default
 - YAML cache system. Yields faster loading times after first game start.
 - wrapper around pdb's set_trace
 - BuildingCollectors can have no home building

Modified structures
 - removed our center_widget, now use pychan's `position_technique="automatic"`
   and modified positioning code to use this shortcut for "center:center"
 - custom tooltip widgets now support names set in python code
 - renamed `unknownhorizons.mo` to `unknown-horizons.mo` (usage of `%name`)
 - unknown-horizons.mo now found in `content/lang/` (was: `build/mo/`)
 - try to use installed pyenet version before searching for compiled one
 - rename build menu icons to achieve unified naming convention
 - roads on field layer instead of ground layer (simplifies rendering)
 - minimap now based on fife.Image (was: Point). Introduces zoom problems
   which are fixed in the development branch of FIFE, ETA next UH release.
 - basic styling for all widgets via load_uh_widget
 - not store hard references to any gui file anymore
 - new changelog formatting
 - moved fife path setup into own function, run_tests uses this now
 - doubled speed of get_random_location by seldomly finding invalid positions
 - only try random jobs for animals

Fixed crashes and inconsistencies
 - fixed save/load of scenario variables
 - properly destruct the messagewidget
 - pirate had acquired teleportation abilities
 - bug in pirate code: wrong rect calculation
 - trader name was not properly reset
 - crash when saving when there were no saved games
 - crash when deleting trade routes
 - huge memory leak when rotating the minimap
 - abort UH if an invalid fife-path has been specified at command line
 - menu closes correctly on instance removal (delete instance ref)
 - move_home checks now if a unit is already at home
 - avoid freezes due to too little cpu power if game speed is high
 - fix several problems with build-related-fields tab
 - Mac-specific error when defaultlocale was None. Use 'en' as fallback.
 - several crashes when collectors were deleted
 - crashes when removing hunter and farm
 - minimap forgot about islands when settling there
 - shipnames and citynames tables now use same restriction names
 - wrong state was set when a collector had been canceled
 - collectors calculated paths twice
 - crash when a ship was being built
 - crash when a scenario was won
 - crash when loading a scenario savegame
 - check for blocked paths for ships caused problems
 - RouteConfig and ProductionOverview disappeared due to garbage collection
 - movement now correctly started after loading


### User-Contributed Content

Translations
 - glossary translations with all important terms (terminology)
 - new translations: bg, cs, fi, hu, lt
 - new terminology translations: cs, da, de, es, fi, fr, nl, pl, pt,
   pt_BR, sl
 - new tutorial translations: fi, pt, ru
 - updates to translations: ca, de, es, et, fr, it, nb, nl, pl, pt,
   pt_BR, ru, sl
 - updates to tutorial translations: de, fr, it, nl

Campaigns and scenarios
 - add scenario 'sc1' by Court-Jus
 - add scenario 'sc2' by Court-Jus
 - add scenario 'sc3' by Court-Jus

Media Content
 - a lot of new city and ship names
 - ( http://forum.unknown-horizons.org/viewtopic.php?t=494 )

New team members with this release, Annotations
 - Push access was granted to:
   Court-Jus, gscai, mihaibivol, squiddy
 - We accepted pull requests or patches by:
   hoffi, sids_aquarius
 - Translators that joined our teams and contributed several strings:
   Please refer to the credits!
 - Special thanks to kurtisevan for holding the weekly challenge
   "More Variety" at [Open Game Art](http://opengameart.org)!


- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -

2011-04-16: Milestone 2011.1
----------------------------
changelog date: APR 16; rev: 3e0151a23dbd0de8b4ac6c697099963eeb59abc7

* General
  - New: UH DFSG compatible, ready for inclusion in e.g. official debian repo
  - New: enet for darwin-x64 => MP possible on mac as well
  - New: Implemented placement and save/load of fish tiles
  - New: Keep statistics about how many res have been produced at a settlement
  - New: Introduced a simple way to create special change listeners
  - New: scenario conditions related to production of resources and units
  - New: settlement now has a list of buildings for each type
  - New: xml loading method, using filename as widget name
  - New: New flags for production lines, enhanced output in print_db_data.py
  - New: Added several comments to xml files
  - New: Tooltips no longer need `\n` hard coded
  - Change: Use `\n` optionally to force a newline in tooltips
  - Change: xml widget file names have to be unique
  - Change: Using show_popup method instead of own xml files for popups
  - Change: Refactored resource display when hovering settlements
  - Change: Refactored mechanism that notifies if production is finished
  - Change: Removed deprecated ProductionFinishedListener and on_remove handle
  - Change: Harmonized callbacks, now use horizons.util.Callback everywhere
  - Change: Detection of exact matches with map file autocompletion in command
            line interface (`--start-map` `--start-campaign` `--load-map`)
  - Change: Capitalized resource names
  - Change: Renamed runin to run_in
  - Change: Renamed all occurences of 'campaign' to 'scenario'
  - Change: Separated popup creation and display in show_popup
  - Change: show_popup is used everywhere in our code now
  - Change: Improvements to the buildtool
  - Change: added is_selectable attribute to concreteobject
  - Change: Removed old, unmaintained pathfinding tests
  - Change: Moved outdated documentation files to misc repository
  - Change: 1024x768 is current minimum resolution
  - Change: Multiplayer lobby now also displays mismatching games and displays
            this, option to disable
  - Change: Disabled pychan debug mode by default
  - Fix: Re-introduced svn legacy code for easier Win snapshots since github
         provides repositories as svn if desired => same client for FIFE and UH
  - Fix: Game did not start with an umlaut/special character in settings.xml
  - Fix: Updated string extraction script to dynamic widget loading
  - Fix: minor issue concerning the creation of random islands
  - Fix: issue with quick- and autosaving
  - Fix: crash when pausing boatbuilder
  - Fix: crash when activating a mine that has already run out of resources
  - Fix: crash when building clay pit or iron mine
  - Fix: crash when clicking on units that are not selectable
  - Fix: crash when saving a game where a fisher ship's home building got demo-
         lished while the ship was outside of it
  - Fix: crash when building a fisher
  - Fix: crash when building branch office
  - Fix: crash when building branch office from ship after fisher was selected
  - Fix: bug with the removed non-buildable trees
  - Fix: possible source of bugs that can occur when saving moving units
  - Fix: crash when collectors got cancelled while heading home
  - Fix: Saving from main menu now properly handles errors
  - Fix: uh-builder script works again

* Gameplay and Balancing
  - New: animals no further reproduce when over-populating an island
  - New: Save remaining part of month for buildings for paying running costs
  - New: Map rotation with , and . keys
  - New: hotkey L for displaying or hiding logbook ingame
  - New: Cam focuses selected group (Ctrl-[num] to group, [num] to select)
  - New: Single non-player units can be selected via dragging
  - Change: Buildings can be grouped
  - Change: default value of transfer amount in trade tab now is 50t
  - Change: islands on map get amount of mountains and clay deposits
  - Change: Collectors can only pick up goods at mine entrance
  - Change: Fish deposit now 1x1 (was 3x3)
  - Change: Smeltery now 4x4 (was 3x3)
  - Change: Charcoal burning now 2x3 (was 4x2)
  - Change: Distillery running costs now 10/5 (was 20/10)
  - Change: Tavern running costs now 5/0 (was 0/0)
  - Change: inhabitants at level Settlers
            consume 1 food per 75 seconds (was 60) and
            produce 12 happiness (was 13) and
            produce 5 happiness per education (was 3)
  - Change: Temporarily removed our sheep and made pasture produce lamb wool
  - Change: Lamb wool production 50% faster
  - Change: Updated tutorial (fisher)
  - Change: Fisher now uses a boat. Needs fish tiles in range to produce food.
  - Change: Fisher boat no longer is selectable
  - Change: Fisher boat can drive through shallow water (coastline)
  - Change: selecting a fisher only highlights fish swarms in range, no island
            or sea / water tiles
  - Change: Boatbuilder now produces a (useless) fisherboat
  - Fix: Constructing trails through several buildings not possible anymore
  - Fix: minor bug concerning decommissioning
  - Fix: signal fire was not selectable
  - Fix: tabs of tabwidget blocked large area (width 50 px) all over the screen
  - Fix: Taxes no longer start at 0 when a game is loaded
  - Fix: animals can no longer be handled by two collectors simultaneously
  - Fix: collectors can now reach each building in displayed range
  - Fix: settlers not being able to level up

* Graphics and GUI
  - New: tooltips for resources in buysell tab
  - New: graphics for our fish resource tile.
    Thanks @ [Open Game Art](http://opengameart.org)!
  - New: many icons for build menu and resources
  - New: build menu tab-icons for increments 3 to 6
  - New: updated increment graphics for pavilion
  - New: updated increment graphics for signal fire
  - New: building graphics for charcoal burning
  - New: building graphics for several mountains
  - New: building graphics for iron mine
  - New: building graphics for distillery
  - New: building graphics for smeltery
  - New: building graphics for toolmaker
  - New: building graphics for pasture
  - New: placeholders for all buildings of increment 3 we have no assets for
  - New: unit 'inhabitant male'
  - New: unit 'inhabitant male 2'
  - New: unit 'hunter'
  - New: unit 'carrier'
  - New: unit 'fisher boat'
  - New: boatbuilder preview images for our current fisher boat
  - New: inactive icons if no logbook navigation possible in this direction
  - New: attack cursor
  - New: Replaced 'Chime the bell' with widget that informs about how everybody
         can contribute
  - New: Added slider value display
  - New: Scrolling through savegames updates Save Details
  - New: minimap rotation with setting
  - New: introduced xml shortcuts for some TooltipButtons and background Icons
  - Change: Retouched many icons for build menu and resources
  - Change: building graphics for brickyard now animated
  - Change: animation time for signal fire
  - Change: selecting buildings only create outline around building instead of
            fully coloring it
  - Change: Don't show trees that are not buildable in build preview
  - Change: Disabling focus for widgets that shouldn't be focusable
  - Change: Sailors build menu 50 px bigger to better fit the other tabs
  - Change: display 'nothing' resource icon in buysell slots by default
  - Change: boatbuilder displays current progress if production is paused
  - Change: save-related settings now sliders instead of listboxes
  - Change: Centered settings window
  - Change: altered text wrap behaviour in tooltips
  - Change: Allow more than one headline per widget
  - Change: Ingame menu and Main menu are more similar
  - Change: Modified default style
  - Fix: Made \n in tooltips be recognized again
  - Fix: Load correct graphics for buildings with versions differing from
         increment to increment
  - Fix: display of production lines with multiple input or output resources

* Translations
  - New: tutorial translations: Dutch, Italian, French
  - New: translations: Russian, Slovenian
  - New: simple script to compile translations on Windows.
         Needs msgfmt in $PATH.
  - New: Translate difficulty, author, description in create_scenario_pot.sh
  - New: Allows translation of all scenarios in create_scenario_pot.sh
  - Change: Added sorted() call to ensure small guitranslations.py diffs
  - Change: Updated labels to achieve unified spelling style
  - Change: Updated translation template
  - Change: Updated almost all translations

* Audio
  - New: two completely new gameplay tracks
  - New: one remastered gameplay track
  - Change: Replaced build.ogg by own file licensed under CC-BY-SA 3.0
  - Change: Replaced ships_bell.ogg by a file licensed under CC-0
  - Change: hazure relicensed our lumberjack sounds under CC-BY-SA 3.0
  - Change: Moved license file for sounds to main LICENSE

... and a lot more smaller bugfixes as well as improvements.

- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -

2010-09-17: Milestone 2010.1
----------------------------
* General
  - New: tutorial
  - New: start german docbook manual
  - New: introduced scenarios and captains log
  - New: Updated a bunch of documentation and updated the incode tutorial
  - New: Implemented support for changing building gfx (any building) on
         increment upgrade. (autoupgrade).
  - New: Tried to make storage collectors more intelligent by making them
         prefer pickups at buildings whose inventory is full.
  - New: Add `--version` option to run_uh.py
  - New: applied some optimization to the buildingtool
  - New: Expanded UhDbReader
  - New: This adds i18n support to setup.py
  - New: Do not require a restart for toggling sound
  - New: Limited the messagewidget to 5 messages max on screen
  - New: Game now pauses when logbook is shown
  - New: community resource icon
  - New: inhabitant tab of the marketplace
  - New: Included system info in debug output
  - New: multiplayer
  - New: Print to log why systemwide fife can't be imported, if so. (usually,
         it will say 'not found', but in some cases, there could be other
         import issues, where the error message can be of some help)
  - New: Added commandline flag to restore the default settings:
         `--restore-settings`
  - New: Pressing enter in a change name dialog (for ship or settlement) now
         acts as submit button
  - New: Applied patch by Yeya to improve random map generation
  - New: Game will now create a settings.xml file on first program launch
         containing the new settings, it's now used instead of the old sqlite
         database
  - New: Added community ressource as requirement for settlers
  - New: Marketplace now produces the community resource
  - New: add `--mp-master` commandline option. Syntax:
         `--mp-master=ip:port` or `--mp-master=ip (+ default port)`
  - New: Extend .bat to use debug with `--debug`, default is still non debug
  - New: Included system info in debug output
  - New: better description for `--mp-bind`
  - New: don't import fife from global python module path if
         `--fife-path` is set
  - New: (savegame revisioning patch) closed by dario
  - New: updated help to include chat hotkey
  - New: create new traders when there are many settlements
  - New: Implemented the pause/resume production button for the boatbuilder
  - New: Add a QuickLoad per keystroke while in the main menu F9
  - New: Use full, native, language names in the settings dialog
  - New: Made highlighting buildable tiles about twice as fast
  - New: Made rect.get_radius_coordinates() at least 2 to 4 times faster
  - New: Made building radius preview (the yellow stuff) about 30% faster
  - New: Added claypit to the game
  - New: Made clay pit produce clay
  - New: Made bricks collected by the storage
  - New: Increase savegame version
  - New: F9 in mainmenu will quickload now
  - New: Increase generator for randommaps
  - New: bash based uh-builder script
  - New: Add important screen resolutions
  - Change: Tents are now in lvl 1 when built
  - Change: Improve autoscroll, should increase the performance
  - Change: Increase the deep water tile size by a factor of 10. Should
            improve performance quite a bit, especially when above water
  - Change: Removed Settings class in favor of the new fife_settings module
  - Change: All settings are now managed by the new extension
  - Change: Some settings have been moved to the constants, like View and Tick
            settings
  - Change: Made textiles a level 2 requirement instead of level 1
  - Change: moved farm, weaver, pasture, potatofield to 2nd increment
  - Change: rearranged build menu
  - Change: Rename cannonboat to huker
  - Change: Refactored engine sound management code
  - Change: Toggling sound on/off no longer requires reboot
  - Change: Reworked directory structure for new tile and path sets
  - Change: make UH version string using git revisions
  - Fix: Workaround: Disabled middle mouse button scrolling
  - Fix: Added layer for fields fixes #521
  - Fix: fixed segfault caused by quitting UH while preloading thread is
         active
  - Fix: Empty city or ship name make problems
  - Fix: added patch from cubathy, Bug when switching language
  - Fix: Fixed bug that allowed you to build fields over each other
  - Fix: Fixed setup.py install the unknown-horizons executable into
         `/usr/games`
  - Fix: The attached patch avoids that boats are created at the same place
  - Fix: Stupid hack to make UH work with umlauts in the user dir on windows
  - Fix: FIXED by FIFE :D  (Doubleclick in menu to confirm)
  - Fix: Game autoscrolls into corner
  - Fix: crash by removing storage tent
  - Fix: Don't crash when loading corrupted save files. Instead give a nice
         error to retry.

* Graphics and GUI
  - New: Added lumberjack building for pioneer increment
  - New: Added gfx for pioneers house
  - New: Added a second pioneers house
  - New: Added school model for pioneers
  - New: Added new level 2 farm model
  - New: Added Clay Pit gfx
  - New: Added a building and resource tree made
  - New: Added clay resource
  - New: Added brickyard
  - New: Added multiplayer lobby with chat and ingamechat
  - New: Added new weaver model, and moved from sailors to pioneers
  - New: Added an overview tab to the signal fire
  - New: Display a tab when clicking on resource deposit
  - New: Added new player emblems
  - New: Trader got an own overview tab
  - New: add global storage display to the ships inventory
  - Change: Credits are now splitted into multiple pages with tabs
  - Change: Logbook now flips pages like a real book
  - Change: New boat builder tab
  - Change: Replaced as_pirate0 with new gfx set (armed sloop)
  - Change: Updated several build menu icons
  - Change: Slightly re-ordered settings menu

* Sound
  - New: Theme by novatlan

* Translations
  - New: Added Catalan; Valencian translation
  - New: Added Portuguese (Brazil) translation
  - New: Added Spanish; Castilian translation
  - New: Added Estonian translation
  - New: Added Italian translation
  - Change: Updated English translation
  - Change: Updated German translation; added German tutorial
  - Change: Updated Polish translation
  - Change: Updated French translation

... and a lot more smaller bugfixes.

- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -

2009-10-18: Milestone 2009.2
----------------------------
* General
  - New: The game creates logfiles now. You can find them in your user folder
         in `.unknown-horizons/log/`
  - New: Wild animals graze on the islands
  - New: Hunters tent which produces food from wild animals
  - New: Added a function to load a map directly via the command line
  - New: The free trader will only visit your settlement if you place a signal
         fire near your branch office
  - New: Some new minor options in the market place menu
  - New: Allow changing the tax rate
  - New: It's now possible to change the name of your ship or settlement
  - New: Started implementing the second settlement level: settlers
  - New: Added potato field as food source
  - New: Working autosave function
  - New: Implemented autorotate for buildings on coastlines
  - New: The ship is now placed randomly
  - New: If the settlers happiness falls below a specific level, the tent
         changes to a ruin
  - New: Implemented a players name and color
  - New: Added a school (no graphic at the moment)
  - New: Added sugar fields (no graphic at the moment)
  - New: Added a few messages that inform the player about different grievances
  - New: Started work on random maps
  - New: Started work on the scenario system
  - New: Implemented a mini tutorial
  - New: Added account tab for main square which shows the financial overview
         of the settlement
  - New: Fade out nearby buildings and trees while building
  - New: System for settlers happieness, consumation and taxation
  - Change: The game uses bigger water-tiles now to improve the performance
  - Change: Completely changed the farm system: There is only one farm building
            which can cultivate any kind of field including sheep-runs
  - Change: Screenshots are now saved into the users folder
  - Fix: Changing the colordepth to 32 Bit works now without a crash
  - Fix: Many code and speed optimizations in general
  - Fix: The savegames work properly now (small trees, …)
  - Fix: Player ship got stuck on the left lower side of the map in some cases
  - Fix: Changed some stuff relating to the translation
  - Fix: Fixed temporary freeze if the player tried to send a ship onto land

* Graphics and GUI
  - New: Added tooltips
  - New: Button to resume a paused game in the pause menu
  - New: Button to switch to destruction mode
  - New: Added a clickable minimap
  - New: Added graphics for potato field and pasture
  - New: Added message buttons for different kinds of messages
  - New: Added graphic for tent ruin
  - New: Highlight the currently selected quantity of goods in exchange menu
  - New: Gamespeed is now displayed in the upper right corner
  - New: Added icon for farm and potato field
  - Change: Disabled the inventory of settlers
  - Change: Changed the style of the pause menu
  - Change: Improved building graphics of Church and Farm
  - Change: Rearanged the building menu
  - Change: Changed some other GUI menus
  - Change: Added a production line with a button to disable production
  - Change: Changed buttons for selecting quantity in exchange menu
  - Change: Unused required ressource icons in ressource bar are now hidden

* Sound
  - New: Added ambient sounds for chapel and fisher
  - New: Added sound when founding a new settlement
  - New: Added sound when winning a mission

* Translations
  - New: Added polish translation
  - Change: Updated some translation files
  - Change: Changed some volume settings

... and a lot more smaller bugfixes.

- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -

2009-07-08: Milestone 2009.1
----------------------------
* General
  - New: Boadbuilder class with unitcreation, it's possible to build ships
  - New: Support for translating the whole GUI was added, including
         German, French, Portuguese and Norwegian translations
  - New: menu to choose language in settings
  - New: Load/save function for maps
  - New: Start work at wildanimals
  - New: Random start position for playership
  - New: add commandline arguments `--start-map` and `--enable-unstable-features`
  - New: Add logging system
  - New: Add debug modul option for commandline `--debug-module`
  - New: debug messages are now only shown by using `./run_uh.py -d`
  - New: Add new tabwidget
  - New: Ship radius when building is now updated on the fly if the ship moves
  - New: Manpage
  - New: Change Style of the mainmenu and all submenus
  - New: Add Developermap with only one small island
  - New: Translations in Portuguese Norwegian German French
  - Change: Hotkeys: set g for grid, b for buildmenu and d for debugger
  - Fix: Building speed has been improved, lumberjack preview is now
         almost lagfree
  - Fix: Loading speed has been improved
  - Fix: Tearing buildings no longer crashes the game
  - Fix: All exceptions when ending a session have been taken care of
  - Fix: Fixed trading bug; selling resources now gives you money
  - Fix: building multiple streets with one click
  - Fix: Main menu doesn't disappear when loading a game

* Graphics and GUI
  - New: Completly new ingame GUI
  - New: Graphics for boat builder
  - New: Graphics for hunter
  - New: Two new variations for inhabitants
  - New: Second model for inhabitants tent
  - Change: Little update on main square
  - Change: Slightly retouched cursor graphics
  - Change: Look of help and creditsmenu

* Sound
  - New: Main theme by Tobias Escher

... and a lot more smaller bugfixes.

- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -

2009-03-08: Milestone 2009.0
----------------------------
* General
  - New: Added a free trader that sells and buys the players goods
  - New: Buildings are now rotatable
  - New: Buy/Sell menu
  - New: Add running costs and an option to decomission buildings to the game
  - New: Started basic work on Gettext support for adding different languages
         to the game
  - New: Isles get filled randomly with trees on startup
  - New: New Map
  - Change: Changed name from OpenAnno to Unknown Horizons
  - Change: Rebuilt ship inventory
  - Change: Random tree/building on build
  - Change: Lumberjack cuts trees randomly
  - Change: Massive changes in the content directory structure to allow easier
            implementation of animations
  - Fix: Crash in build mode
  - Fix: Collectors use tents as path
  - Fix: Crash in Destruction mode - mouse drag
  - Fix: Trees being build over existing sreets and trees autotearing them down
  - Fix: Herder goes backwards and his sheeps are all at the same place
  - Fix: Turning menu: picture and building are asynchron
  - Fix: Stock don't increase after building a storage tent
  - Fix: Weaver steal in other weaver's tent
  - Fix: Resource transfer crashes game when out of range
  - Fix: Buildable status only updated on mouse move

* Graphics and GUI
  - New: New building main square, where inhabitants get their resources
  - New: Icons for switching game speed
  - New: New model for signal fire
  - New: New models for different types of trees
  - Change: Resized buildings and units
  - Change: Added new graphics for units
  - Change: New graphics for main ship and trader
  - Change: Redesign of build menu, added icons of buildable objects
  - Change: New tileset
  - Change: Unified lighting on renderings
  - Change: Updated Buildings: Softened shadows, added some grass, texture work
  - Fix: ship-trademenu and mainmenu are overlapping
  - Fix: Unified lighting in renderings

* Sound
  - New: Implemented build sound
  - New: ambient sounds for lumberjack, herder, main square and branch office
  - New: Rolloff function for sound, which fades ambient sounds depending on
         the position on the map
  - New: New Song Beware the Ship's Kobold!
  - New: Functionality to adjust volume level for music and effects
  - New: Implemented event based speech output
  - New: Added four different sounds to welcome you on the map

... and a lot more smaller bugfixes.

Many thanks go to all contributors, developers, patchers, testers, translators
and supporters.
