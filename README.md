# Alfred Workflows

My collection of [Alfred 5](https://www.alfredapp.com/powerpack/) workflows. Double-click a workflow in [workflows](workflows) to import it, then fill in its [Workflow's Configuration](https://www.alfredapp.com/help/workflows/user-configuration/).

## ButterflyMX

Create a ButterflyMX delivery pass

### Setup

Requires [Home Assistant](https://www.home-assistant.io) with the [ButterflyMX integration](https://github.com/dkmcgowan/ha-butterflymx).

### Usage

Create a single-use delivery pass and copy its PIN via the `bmx` (or `butterfly`) keyword. Add a name to label the pass in the building's access log, e.g. `bmx Amazon`; it defaults to "Delivery".

![ButterflyMX](images/bmx.png)

To copy a message for the delivery driver instead of the bare PIN, set the Clipboard Template in the [Workflow's Configuration](https://www.alfredapp.com/help/workflows/user-configuration/).

## Elgato Key Light

Control your Elgato Key Light

### Usage

Turn the Elgato Key Light on or off via the `elgato` (or `light`) keyword.

![Elgato Key Light](images/elgato.png)

Add `b1` to `b9` to set the brightness from dark to bright, e.g. `elgato b9`.

Add `t1` to `t9` to set the color temperature from 7000K (daylight) to 2900K (soft white), e.g. `elgato t5`.

## Nuki

Lock or unlock the Nuki Smart Lock

### Setup

Requires a Nuki Smart Lock with built-in Wi-Fi. In the Nuki app, enable [MQTT](https://developer.nuki.io/t/mqtt-api-specification-v1-3/17626), including "Allow locking actions".

### Usage

Lock or unlock the door via the `nuki` (or `door`) keyword. Lock Nuki always comes first; type to narrow the list down, e.g. `nuki un`.

![Nuki](images/nuki.png)

Both subtitles show what the lock last reported and how long ago, e.g. "Nuki says: Locked · 3m ago · Battery 63%", and update live while Alfred is open.

The lock only reports when something changes, and can be slow to do so over Wi-Fi, so right after you lock or unlock it the subtitle may still show the old state. Until the lock confirms your command, the subtitle says so, e.g. "Lock sent 12s ago, not confirmed yet".

## OTP

Type the OTP from the latest SMS

### Setup

Give Alfred Full Disk Access in System Settings → Privacy & Security, so it can read Messages.

### Usage

Type the OTP from the latest SMS or RCS message of the last 15 minutes into the frontmost app and press Return via the `otp` (or `2fa`) keyword or the [Hotkey](https://www.alfredapp.com/help/workflows/triggers/hotkey/), set to <kbd>⌃</kbd><kbd>⌘</kbd><kbd>O</kbd>.

![OTP](images/otp.png)

## Pastebin

Upload text from the clipboard to Pastebin

### Setup

Requires a [Rustypaste](https://github.com/orhun/rustypaste) server.

### Usage

Upload the clipboard text and copy its link via the `pb` (or `paste`) keyword.

![Pastebin](images/paste.png)

## URL Shortener

Shorten the URL of the active browser tab

### Setup

Requires a [Chhoto URL](https://github.com/SinTan1729/chhoto-url) server.

### Usage

Shorten the URL of the active tab in the default browser and copy the short link via the `url` (or `link`, `shorten`) keyword. Works with Google Chrome and Safari.

![URL Shortener](images/url.png)

## Wi-Fi Toggle

Turn the Wi-Fi on/off

### Usage

Turn the Wi-Fi on or off via the `wifi` keyword.

![Wi-Fi Toggle](images/wifi.png)
