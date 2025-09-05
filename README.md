
![web33](https://github.com/user-attachments/assets/de17a353-62f4-46a6-8fe4-68b33a995ff1)

TEF6686 Deemphasis Selector:

# TEF6686 Deemphasis Selector

**TEF6686 Deemphasis Selector** is a client-side plugin for the FM-DX Webserver that allows users to quickly select **deemphasis settings** for the TEF6686 receiver. The plugin remembers the last selection, displays a custom dropdown menu, and sends the correct commands to the hardware via WebSocket.

## Features

- Dropdown with deemphasis values: `50 µs`, `75 µs`, `0 µs`, and `MPX`.
- Remembers last selection in `localStorage`.
- Menu adapts to FM-DX Webserver skin/theme.
- Quick switching without page reload.

How It Works

The plugin creates a dropdown button in the FM-DX Webserver interface.

Clicking the button displays the available deemphasis options.

When a user selects a value:

The button text updates.

The value is saved in localStorage.

The corresponding command is sent to TEF6686 via WebSocket.

Compatibility

Fully compatible with the FM-DX Webserver front-end interface.

Requires an active WebSocket (window.socket) for command transmission.

Non-invasive — does not modify server-side code.

Installation

Save the script as deemphasis-selector.js.

Place it in your FM-DX Webserver plugin directory.

Make sure it is loaded by the web interface (or include via <script> tag if necessary).

License & Credits

This plugin was designed with assistance from ChatGPT for code generation and documentation.

Provided as-is, free for personal and non-commercial use. Attribution appreciated.
