![](imgs/logo.png)

## Welcome to Crapht Box

Click to read this [manual online](https://paladin-t.github.io/crft/docs/manual).

Crapht Box is a Fantasy Physics Sandbox, inspired by the Fantasy Console genre. It brings an authentic world with a number of disks and tools. And leaves you to play, program and share creations.

## Table of content

* Part I. Fundamental
	* [Operations](#operations)
	* [Specifications](#specifications)
	* [Capturing](#capturing)
		* [Screenshot](#screenshot)
		* [GIF](#gif)

* Part II. Crafting
	* [Physics elements](#physics-elements)
	* [Sensor elements](#sensor-elements)
	* [Chip elements](#chip-elements)
	* [Dynamics elements](#dynamics-elements)

* Part III. Programming
	* [Syntax](#syntax)
	* [Directories](#directories)
	* [Basic](#basic)
		* [Basic module](#basic-module)
	* [Standard](#standard)
		* [Collection module](#collection-module)
		* [Coroutine module](#coroutine-module)
		* [Datetime module](#datetime-module)
		* [Image module](#image-module)
		* [IO module](#io-module)
		* [JSON module](#json-module)
		* [Keycode module](#keycode-module)
		<!-- * [Net module](#net-module) -->
		* [OS module](#os-module)
		* [Random module](#random-module)
		* [Web module](#web-module)
	* [Common](#common)
		* [Common module](#common-module)
	* [Elements](#elements)
		* [Physics module](#physics-module)
		* [Rope module](#rope-module)
		* [Particles module](#particles-module)
		* [Electronics module](#electronics-module)
		* [Sensor module](#sensor-module)
		* [Dynamics module](#dynamics-module)
		* [AI module](#ai-module)
		* [Alchemy module](#alchemy-module)
	* [Camera, boxes and history](#camera-boxes-and-history)
		* [Camera module](#camera-module)
		* [Minimap module](#minimap-module)
		* [Toolbox module](#toolbox-module)
		* [Sandbox module](#sandbox-module)
		* [History module](#history-module)
	* [GUI](#gui)
		* [GUI module](#gui-module)
		* [Layout module](#layout-module)
	* [Localization](#localization)
		* [Localization module](#localization-module)
		* [Dictionary module](#dictionary-module)
	* [Utilities](#utilities)
		* [Star module](#star-module)
		* [Prefab module](#prefab-module)
	* [Application](#application)
		* [Application module](#application-module)
	* [Program](#program)
		* [Program module](#program-module)
	* [In-disk](#in-disk)
		* [Disk module](#disk-module)

* Part IV. Editors
	* [Code editor](#code-editor)
	* [Map editor](#map-editor)
	* [Level editor](#level-editor)
	* [Element editor](#element-editor)

* Part V. Sharing
	* [Exporter and importer](#exporter-and-importer)
	* [Submitting](#submitting)
	* [Subscribing](#subscribing)
	* [Unsubscribing](#unsubscribing)
	* [Pushing](#pushing)
	* [Pulling](#pulling)
	* [Forking](#forking)

[HOME](#welcome-to-crapht-box)

# Part I. Fundamental

## Operations

Application:

* `LMB`: confirm
* `Enter`: confirm
* `Escape`: cancel
* `Y`/`N`: yes/no
* `Scroll wheel`: scroll

* `F1`: show this manual
* `F6`: take a screenshot
* `F7`: record frames for GIF
* `F8`: stop GIF recording
* `Alt`+`Enter`: toggle fullscreen

Home:

* `Space`: load a disk

Crafting:

* `LMB`: confirm operations; move camera; or placing, hold `Shift` for continuous placing
* `RMB`: select
* `Scroll wheel`: scroll/zoom

* `Ctrl`+`Z`/`Ctrl`+`Y`: undo/redo
* `Ctrl`+`H`: copy the history, hold `Shift` to escape double quotes
* `Ctrl`+`F`: open the tool search box
* `\`: hide the HUD

* `Ctrl`+`A`: select all
* `Ctrl`+`C`: copy selection
* `Ctrl`+`X`: cut selection
* `Ctrl`+`V`: paste selection
* `Left`/`Right`/`Up`/`Down`: move selection, hold `Ctrl` for partial moving
* `Delete`: delete selection

## Specifications

* Display: down to 640x480, scalable
* Audio: 2 music channels, 4 sound effect channels, 1 speech channel
* Code: Wren, Lua
* Gamepad: 6 buttons (D-Pad + A/B)
* Keyboard and mouse: supported

## Capturing

### Screenshot

Press `F6` to take a screenshot, it prompts to save it to your local storage.

### GIF

Press `F7` to record frames for GIF, press `F8` to stop GIF recording, it prompts to save it to your local storage.

[HOME](#welcome-to-crapht-box)

# Part II. Crafting

## Physics elements

<!--
"phy/box"
"phy/sphere"
"phy/pyramid"
"phy/slope"
"phy/wheel"
"phy/focus"
"phy/bouncy_box"
"phy/bouncy_sphere"
"phy/bouncy_pyramid"
"phy/bouncy_slope"
"phy/static_box"
"phy/static_sphere"
"phy/static_pyramid"
"phy/static_slope"
"phy/iron_box"
"phy/iron_sphere"
"phy/iron_pyramid"
"phy/iron_slope"
-->

The physics category contains regular rigid bodies in a few shapes. Physics does not take any role in a circuit, but it does being framework in the physical scene. See tooltips in application for details.

## Sensor elements

<!--
"snsr/btn"
"snsr/btnp"
"snsr/toggle"
"snsr/touch"
"snsr/touchp"
"snsr/touch_relay"
"snsr/touchp_relay"
"snsr/cross_gate"
"snsr/contact_gate"
"snsr/gravity"
-->

The sensor category contains gamepad input, mouse/touch input, in-scene interactable sensors, etc. Sensor can be used as signal source in a circuit. See tooltips in application for details.

## Chip elements

<!--
"chip/constant_byte"
"chip/constant_ascii"
"chip/randomizer_byte"
"chip/pulse"
"chip/register"
"chip/accumulator"
"chip/relay"
"chip/delay"
"chip/fuse"
"chip/trigger_edge"
"chip/trigger_difference"
"chip/wire_i"
"chip/wire_l"
"chip/wire_y"
"chip/wireless_sender"
"chip/wireless_receiver"
"chip/dot"
"chip/led"
"chip/ascii"
"chip/ssd"
"chip/decoder_num2ssd"
"chip/neg"
"chip/add"
"chip/sub"
"chip/mul"
"chip/div"
"chip/mod"
"chip/abs"
"chip/eq"
"chip/neq"
"chip/lt"
"chip/leq"
"chip/gt"
"chip/geq"
"chip/and"
"chip/or"
"chip/not"
"chip/xor"
"chip/band"
"chip/bor"
"chip/bnot"
"chip/bxor"
"chip/lshift"
"chip/rshift"
"chip/environment_now"
-->

The chip category contains signal generators, conductors, logic circuits, etc. Chip can be used as signal source, intermediate node or output reactor in a circuit. See tooltips in application for details.

## Dynamics elements

<!--
"dyn/jet"
"dyn/rocket"
"dyn/airscrew"
"dyn/tnt"
"dyn/motor"
"dyn/crawler_belt"
"dyn/rifle"
"dyn/shotgun"
"dyn/flamethrower"
"dyn/laser"
"dyn/electromagnet"
"dyn/spider_silk"
"dyn/hydropress"
"dyn/escapement"
"dyn/catcher"
"dyn/tone_square"
-->

The dynamics category contains power sources, weapons, etc. Dynamics can be used as output reactor in a circuit. See tooltips in application for details.

[HOME](#welcome-to-crapht-box)

# Part III. Programming

## Syntax

Crapht Box uses the [Box2D](http://box2d.org/) engine for physics simulation.

Disk in Crapht Box is mainly programmed in the [Wren](http://wren.io/) programming language.

<!--
_Experimental: It is also possible to program in the [Lua](http://www.lua.org/) programming language, using the [B95](https://github.com/paladin-t/b95) compiler implemented in Wren._
-->

## Directories

All data and editable disks are stored in a library directory on local storage. The root path of `${Documents}` is:

* "C:/Users/YourName/Documents/Crapht Box/" on Windows
<!--
* "/Users/YourName/Documents/Crapht Box/" on MacOS
* "/home/YourName/Documents/Crapht Box/" on Linux
-->

Lookup priorities for `import`:

| Priority | Directory | Note |
|---|---|---|
| 1 | Built-in | For `Meta`, `Random` |
| 2 | "`${disk}`/content/" | `${disk}` is the current running one |
| 3 | "./shell/content/" | |
| 4 | Falls to reading/writing solvers | |

Reading/writing solvers for IO accessing:

| Prefix | Directory | Note |
|---|---|---|
| "app://" | "./" | The current working directory |
| "disk://" | "`${disk}`/" | `${disk}` is the current running one |
| "doc://" | "`${Documents}`/" | |
| - | - | Can be relative or absolute path |

## Basic

### Basic module

**Class `Basic`**

* **static** `callRoutine(func [, ...])`

* **static** `retainValue(name, val)`
* **static** `releaseValue(name)`

* **static** `clip()`
* **static** `clip(x, y, w, h)`
* **static** `text(x, y, txt, col)`
* **static** `text(x, y, txt, col, isutf)`
* **static** `plot(x, y, col)`
* **static** `line(x0, y0, x1, y1, w, col)`
* **static** `circ(x, y, r, col)`
* **static** `circfill(x, y, r, col)`
* **static** `ellipse(x, y, rx, ry, col)`
* **static** `ellipsefill(x, y, rx, ry, col)`
* **static** `arc(x, y, r, sa, ea, pie, col)`
* **static** `arcfill(x, y, r, sa, ea, pie, col)`
* **static** `rect(x0, y0, x1, y1, col)`
* **static** `rectfill(x0, y0, x1, y1, col)`

* **static** `sget(sprite, x, y [, frame])`
	* `frame`: defaults to 0
* **static** `sset(sprite, x, y, val [, frame])`
	* `frame`: defaults to 0
* **static** `mget(map, x, y [, layer])`
	* `layer`: defaults to 0
* **static** `mset(map, x, y, val [, layer])`
	* `layer`: defaults to 0
* **static** `iget(quantized, x, y)`
* **static** `iset(quantized, x, y, val)`
* **static** `tget(truecolor, x, y)`
* **static** `tset(truecolor, x, y, val)`

* **static** `btn(k)`
* **static** `btnp(k)`
* **static** `key(k)`
* **static** `keyp(k)`
* **static** `touch()`
* **static** `touch(key)`
* **static** `touchp()`
* **static** `touchp(key)`
* **static** `touchm()`

* **static** `play(seq, channel, preset, loop)`
* **static** `stop(channel)`

* **static** `say(words [, speed, pitch, throat, mouth])`
	* `speed`: defaults to 72; with range of values from 0 to 255
	* `pitch`: defaults to 64; with range of values from 0 to 255
	* `throat`: defaults to 128; with range of values from 0 to 255
	* `mouth`: defaults to 128; with range of values from 0 to 255

**Class `Terminal`**

* **static** `show()`
* **static** `hide()`

* **static** `write(t)`
* **static** `write(t, c)`
* **static** `write(t, r, g, b, a)`
* **static** `writeLine(t)`
* **static** `writeLine(t, c)`
* **static** `writeLine(t, r, g, b, a)`
* **static** `backspace()`
* **static** `deleteLine()`
* **static** `clear()`

**Class `Resource`**

* `construct load(path)`
* `construct load(type, width, height)`
* `construct load(type, width, height, n)`
* `unload()`

* `count`

* `width`
* `height`

## Standard

### Collection module

**Class `Stack`**

* `construct new()`
* `construct new(threshold)`

* `isEmpty`

* `peek`

* `push(val)`
* `pop()`

**Class `Mapper`**

* **static** `merge(...)`

* **static** `mustBe(obj, k)`
* **static** `mayBe(obj, k, fall)`

### Coroutine module

**Class `Coroutine`**

* `construct new()`

* `isEmpty`

* `clear()`
* `start(co [, ...])`

* `update(delta)`

### Datetime module

**Class `DateTime`**

* **static** `ticks`

* **static** `now`

### Image module

**Class `Image`**

* `construct new()`

* `[x, y]`
* `[x, y] = (col)`

* `width`
* `height`

* `resize(w, h)`

* `load(w, h)`
* `load(path)`
* `save(path)`

### IO module

**Class `Path`**

* **static** `absoluteOf(path)`

* **static** `parentOf(path)`
* **static** `nameOf(path)`
* **static** `extensionOf(path)`

* **static** `split(path)`
* **static** `concat(patha, pathb)`

* **static** `exists(path)`
* **static** `move(path, target)`
* **static** `copy(path, target)`
* **static** `remove(path [, toTrashBin])`
	* `toTrashBin`: defaults to `true`

* **static** `createFile(path)`
* **static** `createDirectory(path)`

* **static** `getFiles(path, pattern [, recursive])`
	* `recursive`: defaults to `false`
* **static** `getDirectories(path [, recursive])`
	* `recursive`: defaults to `false`

* **static** `explore(path)`

**Class `File`**

* `construct new()`

* `open(path [, write])`
	* `write`: defaults to `false`
* `close()`

* `length`
* `endOfStream`

* `peek`
* `poke(pos)`

* `readAll()`
* `read()`
* `readU8()`
* `readI32()`
* `readFloat()`
* `readString(length)`
* `readLine()`
* `readBytes()`

* `write(data)`
* `writeU8(data)`
* `writeI32(data)`
* `writeFloat(data)`
* `writeString(data)`
* `writeLine(data)`
* `writeBytes(data)`

**Class `FileInfo`**

* `construct new(path)`

* `isEmpty`

* `fullName`
* `parentName`
* `name`
* `extension`

* `exists`
* `create()`
* `remove([toTrashBin])`
	* `toTrashBin`: defaults to `true`
* `moveTo(target)`
* `copyTo(target)`

* `readAll()`

* `parent`

**Class `DirectoryInfo`**

* `construct new(path)`

* `isEmpty`

* `fullName`
* `parentName`
* `name`

* `exists`
* `create()`
* `remove([toTrashBin])`
	* `toTrashBin`: defaults to `true`
* `moveTo(target)`
* `copyTo(target)`

* `getFiles(pattern [, recursive])`
	* `recursive`: defaults to `false`
* `getDirectories([recursive])`
	* `recursive`: defaults to `false`

* `parent`

### JSON module

**Class `Json`**

* **static** `OrderedKey`

* **static** `tokenize(string)`

* **static** `parse(string [, ordered])`
	* `ordered`: defaults to `false`

* **static** `stringify(object [, compact])`
	* `compact`: defaults to `false`

### Keycode module

**Class `KeyCode`**

* **static** `MouseLeft`
* **static** `MouseMiddle`
* **static** `MouseRight`

* **static** `GamepadLeft`
* **static** `GamepadRight`
* **static** `GamepadUp`
* **static** `GamepadDown`
* **static** `GamepadA`
* **static** `GamepadB`

* **static** `Return`
* **static** `Esc`
* **static** `Backspace`
* **static** `Tab`
* **static** `Space`

* **static** `A`~`Z`

* **static** `Num0`~`Num9`

* **static** `F1`~`F12`

See "./shell/content/keycode.wren" for more.

<!--
### Net module

// Not implemented.
-->

### OS module

**Class `Os`**

* **static** `info`

* **static** `clipboardText`
* **static** `clipboardText = (txt)`

### Random module

**Class `Random`**

See [`Random`](http://wren.io/modules/random/random.html) for details.

### Web module

**Class `Web`**

* **static** `surf(url)`

* **static** `request(url [, method [, field]])`
	* `method`: defaults to "get"
	* `field`: defaults to `null`

## Common

### Common module

**Class `Direction`**

* **static** `Left`
* **static** `Right`
* **static** `Up`
* **static** `Down`
* **static** `Any`

**Class `Component`**

* **static** `None`
* **static** `Fixture`
* **static** `Joint`
* **static** `Conduction`
* **static** `Particle`
* **static** `Contact`
* **static** `Target`
* **static** `All`: composited by all above

**Class `Group`**

* **static** `Void`
* **static** `Environment`
* **static** `Player`
* **static** `Ai`
* **static** `All`: composited by all above

**Class `Vec2`**

* `construct new()`
* `construct new(x, y)`

* `toString`

* `x`
* `x = (value)`
* `y`
* `y = (value)`

* `-`
* `+ (other)`
* `- (other)`
* `* (other)`

* `normalize()`
* `normalized`

* `length`
* `lengthSquared`

* `distance(other)`
* `distanceSquared(other)`

* `dot(other)`
* `cross(other)`

* `angle()`
* `angle(other)`
* `rotated(angle)`
* `rotated(angle, pivot)`

**Class `Vec3`**

* `construct new()`
* `construct new(x, y, z)`

* `toString`

* `x`
* `x = (value)`
* `y`
* `y = (value)`
* `z`
* `z = (value)`

* `-`
* `+ (other)`
* `- (other)`
* `* (other)`

* `normalize()`
* `normalized`

* `length`
* `lengthSquared`

* `distance(other)`
* `distanceSquared(other)`

* `dot(other)`
* `cross(other)`

**Class `Vec4`**

* `construct new()`
* `construct new(x, y, z, w)`

* `toString`

* `x`
* `x = (value)`
* `y`
* `y = (value)`
* `z`
* `z = (value)`
* `w`
* `w = (value)`

**Class `Rect`**

* `construct new()`
* `construct new(x, y, w, h)`

* `toString`

* `x`
* `x = (value)`
* `y`
* `y = (value)`
* `width`
* `width = (value)`
* `height`
* `height = (value)`

**Class `Rot`**

* `construct new()`
* `construct new(a)`
* `construct new(s, c)`

* `toString`

* `s`
* `s = (value)`
* `c`
* `c = (value)`

* `angle`
* `angle = (value)`

* `* (other)`

**Class `Color`**

* **static** `Black`
* **static** `White`
* **static** `Red`
* **static** `Green`
* **static** `Blue`
* **static** `Yellow`
* **static** `Orange`

* `construct new()`
* `construct new(r, g, b)`
* `construct new(r, g, b, a)`

* `toString`

* `r`
* `r = (value)`
* `g`
* `g = (value)`
* `b`
* `b = (value)`
* `a`
* `a = (value)`

* `rgba`
* `rgba = (value)`

**Class `Handle`**

* **static** `Invalid`

* `toString`

* `id`
* `isValid`

* `type`
* `type = (value)`

* `category`
* `category = (value)`

* `name`
* `name = (value)`

* `nature`
* `nature = (value)`

* `group`
* `group = (value)`

* `instantiated`

* `operable`

* `queriable`
* `queriable = (value)`

* `joinable`
* `joinable = (value)`

* `conductible`
* `conductible = (value)`

* `contactable`
* `contactable = (value)`

* `platform`
* `platform = (value)`

* `visible`
* `visible = (value)`

* `awake`
* `awake = (value)`

* `position`
* `position = (value)`

* `rotation`
* `rotation = (value)`

* `size`
* `size = (value)`

* `aabb`

* `up`
* `down`
* `left`
* `right`
* `direct(vec)`
* `inverse(vec)`

* `vibrate(interval, amplitude)`

* `resource`
* `resource = (value)`

* `color`
* `color = (value)`

* `renderableRotation`
* `renderableRotation = (value)`

* `renderableHFlip`
* `renderableHFlip = (value)`

* `renderableVFlip`
* `renderableVFlip = (value)`

* `length`

* `play([begin, end [, loop, init]])`
	* `begin`: defaults to -1
	* `end`: defaults to -1
	* `loop`: defaults to `true`
	* `init`: defaults to `true`

* `hp`
* `hp = (points)`

* `conduct([alive])`
	* `alive`: defaults to `true`

* `get(type, key)`
* `get(key)`
* `set(type, key, val)`
* `set(key, val)`

* `bounce`
* `bounce = (rate)`

* `fixedRotation`
* `fixedRotation = (fixed)`

* `linearDamping`
* `linearDamping = (damping)`
* `angularDamping`
* `angularDamping = (damping)`

* `linearVelocity`
* `linearVelocity = (velocity)`
* `angularVelocity`
* `angularVelocity = (omega)`

* `applyForce(force, point)`
* `applyForceToCenter(force)`
* `applyTorque(torque)`
* `applyLinearImpulse(impulse, point)`
* `applyAngularImpulse(impulse)`

* `addFixture(params, shape)`
* `clearFixtures()`

* `destroy()`

## Elements

### Physics module

**Class `WorldParam`**

* **static** `MapLayerScale`

**Class `World`**

* **static** `unit`

* **static** `new(g)`

**Class `Shape`**

* **static** `Circle`
* **static** `Edge`
* **static** `Polygon`
* **static** `Chain`

**Class `Fixture`**

* **static** `density`

**Class `Body`**

* **static** `Static`
* **static** `Kinematic`
* **static** `Dynamic`

* **static** `new(hworld, type, pos)`

**Class `JointParam`**

* **static** `BreakForceSquare`
* **static** `Joint1`
* **static** `Joint2`
* **static** `GroundAnchorA`
* **static** `GroundAnchorB`
* **static** `LocalAnchorA`
* **static** `LocalAnchorB`
* **static** `LocalAxisA`
* **static** `LinearOffset`
* **static** `Target`
* **static** `LowerTranslation`
* **static** `UpperTranslation`
* **static** `LowerAngle`
* **static** `UpperAngle`
* **static** `ReferenceAngle`
* **static** `Length`
* **static** `LengthA`
* **static** `LengthB`
* **static** `Ratio`
* **static** `DampingRatio`
* **static** `FrequencyHz`
* **static** `CorrectionFactor`
* **static** `AngularOffset`
* **static** `MotorSpeed`
* **static** `MaxLength`
* **static** `MaxForce`
* **static** `MaxMotorForce`
* **static** `MaxTorque`
* **static** `MaxMotorTorque`
* **static** `CollideConnected`
* **static** `EnableLimit`
* **static** `EnableMotor`

**Class `Joint`**

* **static** `Unknown`
* **static** `Revolute`
* **static** `Prismatic`
* **static** `Distance`
* **static** `Pulley`
* **static** `Mouse`
* **static** `Gear`
* **static** `Wheel`
* **static** `Weld`
* **static** `Friction`
* **static** `Rope`
* **static** `Motor`

* **static** `new(hworld, type, params)`
* **static** `new(hworld, type, params, options)`
* **static** `new(hworld, type, params, options , refocusOnBroken)`

### Rope module

**Class `RopeParam`**

* **static** `BreakForceSquare`

**Class `Rope`**

// Not implemented.

### Particles module

**Class `Particle`**

* **static** `Water`
* **static** `Zombie`
* **static** `Wall`
* **static** `Spring`
* **static** `Elastic`
* **static** `Viscous`
* **static** `Powder`
* **static** `Tensile`
* **static** `Barrier`
* **static** `StaticPressure`
* **static** `Reactive`
* **static** `Repulsive`

**Class `ParticleSystem`**

* **static** `new(hworld)`
* **static** `new(hworld, gravityScale)`
* **static** `new(hworld, gravityScale, density)`

**Class `ParticleGroupParam`**

* **static** `LifetimeBegin`
* **static** `LifetimeEnd`
* **static** `ColorBegin`
* **static** `ColorEnd`
* **static** `ColorFadingBegin`
* **static** `ColorFadingEnd`
* **static** `Direction`
* **static** `Velocity`
* **static** `CouldCollide`
* **static** `Shape`
* **static** `Radius`
* **static** `Flags`
* **static** `Count`

**Class `ParticleGroup`**

* **static** `new(handle)`
* **static** `new(handle, shape)`

**Class `ParticleEmitter`**

* **static** `emit(hgroup)`

### Electronics module

**Class `CircuitParam`**

Blank.

**Class `Circuit`**

Blank.

**Class `ChipParam`**

* **static** `Value`
* **static** `Switchable`
* **static** `SwitchTo`
* **static** `SwitchFor`
* **static** `Switchmost`
* **static** `Flippable`
* **static** `Flipped`

**Class `Chip`**

* **static** `ConstantByte`
* **static** `ConstantAscii`
* **static** `RandomizerByte`
* **static** `Pulse`
* **static** `Register`
* **static** `Accumulator`
* **static** `Relay`
* **static** `Delay`
* **static** `Fuse`
* **static** `TriggerEdge`
* **static** `TriggerDifference`
* **static** `WireI`
* **static** `WireL`
* **static** `WireY`
* **static** `WirelessSender`
* **static** `WirelessReceiver`
* **static** `ReactorEmitter`
* **static** `ReactorDot`
* **static** `ReactorLed`
* **static** `ReactorAscii`
* **static** `ReactorSsd`
* **static** `DecoderNum2Ssd`
* **static** `AlgebraNeg`
* **static** `AlgebraAdd`
* **static** `AlgebraSub`
* **static** `AlgebraMul`
* **static** `AlgebraDiv`
* **static** `AlgebraMod`
* **static** `AlgebraAbs`
* **static** `CompareEq`
* **static** `CompareNeq`
* **static** `CompareLt`
* **static** `CompareLeq`
* **static** `CompareGt`
* **static** `CompareGeq`
* **static** `LogicAnd`
* **static** `LogicOr`
* **static** `LogicNot`
* **static** `LogicXor`
* **static** `BitwiseAnd`
* **static** `BitwiseOr`
* **static** `BitwiseNot`
* **static** `BitwiseXor`
* **static** `BitwiseLShift`
* **static** `BitwiseRShift`
* **static** `EnvironmentNow`

* **static** `frequency`

* **static** `new(hworld, type, pos)`

### Sensor module

**Class `Sensor`**

* **static** `GamepadDown`
* **static** `GamepadUp`
* **static** `Toggle`
* **static** `TouchDown`
* **static** `TouchUp`
* **static** `TouchDownRelay`
* **static** `TouchUpRelay`
* **static** `CrossGate`
* **static** `ContactGate`
* **static** `Gravity`

* **static** `new(hworld, type, pos)`

### Dynamics module

**Class `Power`**

Blank.

**Class `DynamicsParam`**

* **static** `QuotaCycles`

**Class `Dynamics`**

* **static** `Jet`
* **static** `Rocket`
* **static** `Airscrew`
* **static** `Tnt`
* **static** `Motor`
* **static** `CrawlerBelt`
* **static** `Rifle`
* **static** `Shotgun`
* **static** `Flamethrower`
* **static** `Laser`
* **static** `Magnet`
* **static** `SpiderSilk`
* **static** `Hydropress`
* **static** `Escapement`
* **static** `Catcher`
* **static** `Tone`

* **static** `new(hworld, type, pos)`

### AI module

**Class `Behaviour`**

* **static** `Idle`
* **static** `Chase`
* **static** `Jump`
* **static** `Attack`
* **static** `Escape`
* **static** `Fallen`
* **static** `Dead`

**Class `AiParam`**

* **static** `AwakeDistance`: read, write
* **static** `SleepingDistance`: read, write
* **static** `Behaviour`: readonly
* **static** `Motion`: writeonly

**Class `Ai`**

* **static** `Dweller`
* **static** `Warrior`
* **static** `Archer`

* **static** `new(hworld, type, pos)`

### Alchemy module

**Class `Nature`**

* **static** `None`
* **static** `Solid`
* **static** `Liquid`
* **static** `Gaseous`
* **static** `Plasma`
* **static** `Photic`
* **static** `Metal`: composited by `Nature.Ferromagnetic` and `Nature.Nonferromagnetic`
* **static** `Ferromagnetic`
* **static** `Nonferromagnetic`
* **static** `Lithoid`
* **static** `Wood`
* **static** `Goo`
* **static** `Biotic`: composited by `Nature.Vegetal` and `Nature.Creatural`
* **static** `Vegetal`
* **static** `Creatural`
* **static** `ReducingAgent`
* **static** `OxidizingAgent`
* **static** `Combustible`
* **static** `Ignis`
* **static** `Inert`
* **static** `Active`
* **static** `All`: composited by all above

## Camera, boxes and history

### Camera module

**Class `Camera`**

* **static** `wireframe`
* **static** `wireframe = (value)`

* **static** `following`
* **static** `following = (value)`

* **static** `autoFollow`
* **static** `autoFollow = (value)`

* **static** `movable`
* **static** `movable = (value)`

* **static** `zoomable`
* **static** `zoomable = (value)`

* **static** `vibrate(interval, amplitude)`

* **static** `position`
* **static** `position = (value)`

* **static** `size`
* **static** `size = (value)`

* **static** `pixelsPerUnit`
* **static** `pixelsPerUnit = (value)`

* **static** `toScreen(value)`
* **static** `fromScreen(value)`

### Minimap module

**Class `Minimap`**

* **static** `visible`
* **static** `visible = (value)`

* **static** `mapVisible`
* **static** `mapVisible = (value)`

### Toolbox module

**Class `Toolbox`**

* **static** `visible`
* **static** `visible = (value)`

* **static** `setAvailable(available [, category [, name]])`
	* `category`: defaults to "*"
	* `name`: defaults to "*"

* **static** `instantiate(hparent, category, name, pos, rot [, contactable [, operable [, group]]])`
	* `contactable`: defaults to `false`
	* `operable`: defaults to `false`
	* `group`: defaults to `Group.Environment`

### Sandbox module

**Class `AskParam`**

* **static** `None`
* **static** `IgnoreSensor`
* **static** `IgnoreFixed`
* **static** `InstantiatedOnly`
* **static** `OperableOnly`
* **static** `JoinableOnly`
* **static** `ConductibleOnly`
* **static** `Multiple`
* **static** `Default`: composited by `AskParam.InstantiatedOnly`, `AskParam.OperableOnly` and `AskParam.Multiple`

**Class `Sandbox`**

* **static** `operable`
* **static** `operable = (value)`

* **static** `selectable`
* **static** `selectable = (value)`

* **static** `draggable`
* **static** `draggable = (value)`
* **static** `dragForce`
* **static** `dragForce = (value)`

* **static** `setPlacingRect(rect)`
* **static** `setPlacingSnapToGrid(snap)`
* **static** `setPlacingCanOverlap(ovlp)`

* **static** `setRotatingAxiallyAligned(rot)`
* **static** `setRotatingFree(rot)`

* **static** `filter(hworld, category, name [, options [, group]])`
	* `options`: defaults to `AskParam.Default`
	* `group`: defaults to `Group.All`

* **static** `query(hworld, point, radius [, options [, group [, filter]]])`
	* `options`: defaults to `AskParam.Default`
	* `group`: defaults to `Group.All`
	* `filter`: defaults to `null`

* **static** `raycast(hworld, point1, point2 [, options [, group [, filter]]])`
	* `options`: defaults to `AskParam.Default`
	* `group`: defaults to `Group.All`
	* `filter`: defaults to `null`

### History module

**Class `History`**

* **static** `undoable`
* **static** `undoable = (value)`

* **static** `sealed`
* **static** `sealed = (value)`

* **static** `load()`
* **static** `save()`

* **static** `reload()`
* **static** `unload()`

* **static** `parse(json [, undoable])`
	* `undoable`: defaults to `true`
* **static** `serialize()`

## GUI

### GUI module

**Class `Alignment`**

* **static** `Middle`
* **static** `Left`
* **static** `Right`

**Class `PackingStyle`**

* **static** `None`
* **static** `NineGrid`
* **static** `ThreeGrid`

**Class `CheckBox`**

* `construct new(txt, checked)`

* `readonly`
* `readonly = (value)`

* `value`
* `value = (value)`

* `content`
* `content = (value)`

* `style`
* `style = (value)`

**Class `ComboBox`**

* `construct new()`

* `[index]`
* `[index] = (value)`
* `count`
* `add(item)`
* `insert(index, item)`
* `removeAt(index)`
* `clear()`

* `readonly`
* `readonly = (value)`

* `value`
* `value = (value)`

**Class `IntegerField`**

* `construct new()`
* `construct new(min, max, val)`
* `construct new(min, max, val, step)`

* `readonly`
* `readonly = (value)`

* `value`
* `value = (value)`

* `format`
* `format = (value)`

**Class `RealField`**

* `construct new()`
* `construct new(min, max, val)`
* `construct new(min, max, val, step)`

* `readonly`
* `readonly = (value)`

* `value`
* `value = (value)`

* `format`
* `format = (value)`

**Class `Tab`**

* `construct new()`

* `[index]`
* `[index] = (value)`
* `count`
* `add(item)`
* `insert(index, item)`
* `removeAt(index)`
* `clear()`

* `value`
* `value = (value)`

**Class `Scroll`**

* `construct new()`

* `[index]`
* `[index] = (value)`
* `count`
* `add(item)`
* `insert(index, item)`
* `removeAt(index)`
* `clear()`

* `value`
* `value = (value)`

**Class `Block`**

* `isValid`

* `value`

**Class `MessageBoxButtons`**

* **static** `Ok`
* **static** `OkCancel`
* **static** `YesNo`
* **static** `YesNoCancel`

**Class `DialogResult`**

* **static** `Ok`
* **static** `Yes`
* **static** `OkOrYes`
* **static** `No`
* **static** `Cancel`

**Class `Gui`**

* **static** `screenArea`
* **static** `activeArea`

* **static** `panel(x, y, w, h)`
* **static** `text(content, x, y, w, h [, width, align])`
	* `width`: defaults to 0
	* `align`: defaults to `Alignment.Left`
* **static** `image(content, x, y, w, h [, packing])`
	* `packing`: defaults to `PackingStyle.Normal`
* **static** `tooltip(content, x, y)`
* **static** `link(content, x, y)`
* **static** `button(content, x, y, w, h)`

* **static** `checkBox(ctrl, x, y, w, h)`
* **static** `comboBox(ctrl, x, y, w, h)`
* **static** `integerField(ctrl, x, y, w, h)`
* **static** `realField(ctrl, x, y, w, h)`
* **static** `tab(ctrl, x, y, w, h)`
* **static** `scroll(ctrl, x, y, w, h)`

* **static** `block(timeout)`
	* returns `Block`
* **static** `block()`
* **static** `indicate(target [, size])`
	* returns `Block`
* **static** `indicate()`
* **static** `chat(content)`
	* returns `Block`

* **static** `messageBox(content, buttons)`
	* returns `Block`
* **static** `inputBox(content)`
	* returns `Block`

* **static** `openFileDialog([type [, multiple]])`
	* `type`: defaults to `null`
	* `multiple`: defaults to `false`
* **static** `saveFileDialog([type])`
	* `type`: defaults to `null`
* **static** `pickDirectoryDialog([dir])`
	* `dir`: defaults to `null`

### Layout module

**Class `Container`**

* `construct new()`
* `construct new(f)`
* `construct new(x, y)`
* `construct new(x, y, w, h)`

* `area`
* `offset`
* `step`
* `padding`
* `sameline`
* `active`
* `active = (value)`

* `begin(layout)`
* `end(layout)`

* `refresh()`

**Class `Panel`**

* `construct new(w, h)`

* `step`
* `padding`

* `begin(layout)`

**Class `Flow`**

* `construct new()`
* `construct new(txt)`
* `construct new(txt, ext)`

* `begin(layout)`

* `text`
* `text = (value)`

* `expanded`
* `expanded = (value)`

**Class `Grid`**

* `construct new(hCount, vCount)`

* `step`
* `padding`
* `sameline`

* `begin(layout)`

* `count`

**Class `Layout`**

* `construct new()`

* `isEmpty`
* `peek`
* `push(ctrl)`
* `pop()`

* `inline(w)`
* `newline(h)`

* `with(ctrl)`
* `refresh(ctrl)`

## Localization

### Localization module

**Class `Language`**

* **static** `English`
* **static** `Chinese`
* **static** `Japanese`
* **static** `German`
* **static** `French`
* **static** `Italian`
* **static** `Spanish`
* **static** `Portuguese`

* **static** `fromString(lang)`
* **static** `toString(lang)`

**Class `Localization`**

* **static** `[lang, id]`
* **static** `[lang, id] = (txt)`

* **static** `get(lang, id)`
* **static** `set(lang, id, txt)`
* **static** `remove(lang, id)`
* **static** `clear()`

### Dictionary module

**Class `Dictionary`**

* `construct new()`

* `[id]`
* `[lang, id]`
* `[lang, id] = (txt)`

* `isEmpty`

* `data`

* `get(id)`
* `get(lang, id)`
* `set(lang, id, txt)`
* `remove(id)`
* `remove(lang, id)`
* `clear()`

* `fill(dict)`

## Utilities

### Star module

**Class `Point`**

* `construct new(k, m)`

* `key`

* `message`

* `accomplished`
* `accomplished = (value)`

**Class `Completeness`**

* `construct new(acc, tot)`

* `toString`

* `accomplished`
* `accomplished = (value)`

* `total`
* `total = (value)`

**Class `Star`**

* `construct new(hasVar, getVar, setVar)`

* `[index]`

* `isEmpty`
* `count`

* `stars`

* `indexOf(key)`
* `contains(key)`
* `get(index)`
* `add(key, msg)`
* `clear()`

* `complete(index)`
* `completed(index)`
* `completeness`

* `iterate(iterator)`
* `iteratorValue(iterator)`

### Prefab module

**Class `Fix`**

* **static** `[type]`

* **static** `withNone(hbody, radius, density, options)`
* **static** `withBox(hbody, radius, density, options)`
* **static** `withSphere(hbody, radius, density, options)`
* **static** `withSlope(hbody, radius, density, options)`

* **static** `vertex(data, options)`

**Class `Prefab`**

* **static** `Assets`
* **static** `Entities`

* **static** `new(hworld, name, options)`
* **static** `instantiate(hworld, name, options)`

## Application

### Application module

**Class `Application`**

* **static** `basicAllocatedBytes`
* **static** `wrenAllocatedBytes`
* **static** `vramAllocatedBytes`

* **static** `language`
* **static** `language = (value)`

* **static** `setOption(key, val [, append])`
	* `append`: defaults to `false`

* **static** `exit()`

## Program

### Program module

**Class `Program`**

* `debug`
* `autoPlay`
* `autoPlay = (value)`
* `playing`
* `playing = (value)`
* `played`
* `ended`
* `win([stars [, hypnotize [, tips]]])`
	* `stars`: defaults to `null`
	* `hypnotize`: defaults to `false`
	* `tips`: defaults to `null`
* `lose([stars [, hypnotize [, tips]]])`
	* `stars`: defaults to `null`
	* `hypnotize`: defaults to `false`
	* `tips`: defaults to `null`
* `unlock(disk)`

* `totalEnergy`
* `totalEnergy = (value)`
* `energy`
* `energy = (value)`

* `hasVariable(key)`
* `getVariable(key)`
* `setVariable(key, value)`
* `removeVariable(key)`
* `clearVariables()`

* `addUpdater(signature)`
* `removeUpdater(signature)`
* `clearUpdaters()`

* `loadResource(path)`

* `world`
* `world = (value)`
* `border = (value)`

* `doLoad()`
* `doReload()`
* `doUnload()`

* `doStart()`
* `doQuit()`
* `doResize(width, height)`

* **async** **virtual** `load()`
* **async** **virtual** `reload()`
* **async** **virtual** `unload()`

* **virtual** `start()`
* **virtual** `quit()`
* **virtual** `resize(width, height)`

* **virtual** `gui()`
* **virtual** `update(delta)`

* **virtual** `onCreated(handle)`
* **virtual** `onDeleted(handle)`
* **virtual** `onContacted(handlea, handleb)`
* **virtual** `onLeft(handlea, handleb)`
* **virtual** `onDamaged(hself, hother)`
* **virtual** `onTransfered(handle, newState, oldState)`

* **async** **static** `waitFor(t)`

* **static** `eval(code)`

## In-disk

### Disk module

_This module is experimental._

**Class `Convert`**

* **static** `lineToScene(data)`
* **static** `sceneToLine(data [, snap])`
	* `snap`: defaults to `true`

* **static** `gridToScene(data)`
* **static** `sceneToGrid(data [, snap])`
	* `snap`: defaults to `true`

* **static** `byteCountToString(data)`

**Class `Operate`**

* **static** `create(cmd, index, hworld, built, tagged)`
* **static** `delete(cmd, index, hworld, built, tagged)`
* **static** `move(cmd, index, hworld, built)`
* **static** `rotate(cmd, index, hworld, built)`
* **static** `switchover(cmd, index, hworld, built)`
* **static** `flip(cmd, index, hworld, built)`

* **static** `build(obj, entry, hworld, tagged, onstep)`

**Class `Load`**

* **static** `jsonFile(path [, ordered])`
	* `jsonFile`: defaults to `false`

* **static** `diskInfo()`

* **static** `toolAvailability(data)`

* **static** `world(map, gravity, program)`

* **static** `mapInfo(map, index, fill)`
* **static** `mapPattern(map, index, fill)`
* **static** `mapFixture(map, index, program)`

* **static** `sceneGraph(hworld, data [, onstep])`
	* `onstep`: defaults to `null`

**Class `Storyboard`**

* `construct new()`
* `construct new(dict)`

* `isEmpty`

* `fill(data)`
* `clear()`

* `play(story)`
* `playing`
* `stop()`
* `pend()`
* `pend(p)`
* `update(delta)`

* `iterate(iterator)`
* `iteratorValue(iterator)`

**Class `Stopwatch`**

* `construct new()`
* `construct new(rushtime)`

* `toString`

* `paused`
* `paused = (value)`

* `rushTime`
* `ticks`
* `ticks = (value)`
* `missed`

* `update(delta)`

* `gui()`

[HOME](#welcome-to-crapht-box)

# Part IV. Editors

Crapht Box offers built-in editors to edit entry source code, map, level and element.

## Code editor

Switch to the `Workshop` tab, then click the edit button to edit your creations:

![](imgs/gui/button_edit.png)

The built-in code editor will load the entry source code of the selected disk. To edit other assets, navigate to the directory of a specific disk on your local storage, then use whatever external editors you want for assets.

Notice that you cannot edit readonly disks.

## Map editor

Switch to the `Packs` tab, then load the `Editor/Map Editor` disk. See in-disk help for details.

This editor is for static graphics layers, eg. background, sky, terrain. In the usual case it saves to the "`${disk}`/content/map.map" and "`${disk}`/content/scene.json" file.

## Level editor

Switch to the `Packs` tab, then load the `Editor/Level Editor` disk. See in-disk help for details.

This editor is for static environments, eg. goal, credit, wall. In the usual case it saves to the "`${disk}`/content/scene.json" file.

## Element editor

Switch to the `Packs` tab, then load the `Editor/Element Editor` disk. See in-disk help for details.

This editor is for placing regular elements. In the usual case it saves to the "`${disk}`/content/scene.json" file.

[HOME](#welcome-to-crapht-box)

# Part V. Sharing

You can share your creative disks with the Steam community via Workshop, subscribe to play others' games and programs, and discuss or comment on any creation.

Switch to the `Workshop` tab on the main screen to use following operations.

## Exporter and importer

Click `Export...` for exporting.

Click `Import...` for importing.

Exported disks are standard zip packages.

## Submitting

To submit a new disk to Workshop, select it, then click `Push`.

Use an external editor to modify the "info.json" meta file before pushing as you need. Don't forget to close any external editors that opening the source disk you are going to push, pull, etc.

It's recommended to use a good looking preview, choose a proper genre, and write necessary introduction and notes to help others to get better acquainted with your submission. You could edit submitted information in browser later, including changing description, chaging visibility, updating preview images and videos, etc.

You need to agree to the Steam Workshop's terms of service for submitting.

## Subscribing

Use a web browser to explore the [Crapht Box Workshop](https://steamcommunity.com/app/1227090/workshop/) on Steam to make subscriptions:

![](imgs/workshop_subscribe.png)

All subscribed disks will be automatically downloaded for mounting.

## Unsubscribing

Click `Unsubscribe` on an already subscribed disk in browser or application to stop following it.

## Pushing

When you want to push modifications of a submitted disk, select the disk, then click `Push`.

## Pulling

All subscribed disks are supposed to be updated automatically when Crapht Box boots up, but in case you'd like to check updates manually, just click `Pull`.

## Forking

Click `Fork` to derive from a selected disk.

[HOME](#welcome-to-crapht-box)
