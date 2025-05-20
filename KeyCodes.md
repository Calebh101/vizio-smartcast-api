# Emulating Remote Key Presses

I tried to document all of the valid keys using my TV - and got some neat results. Some entire sets returned FAILURE (I tested up to codeset 15 on those) for some reason.

This is the format: `set.code`. `set` is the codeset of the key, and `code` is the key's code.

For how to use this info, check out [exiva/Vizio_SmartCast_API](https://github.com/exiva/Vizio_SmartCast_API?tab=readme-ov-file#send-remote-control-button-press).

## Set 0 - ASCII

- This set is used to send any ASCII character, including backspace, newline, etc. You have to convert it into ASCII decimal, and use that as your code.

## Set 2 - Transport

- 2.1, 2.6, and 2.7 all appear to rewind (maybe with different speeds) and 2.0, 2.5, and 2.8 all appear to go forward.
- 2.9 appears to pause? But it's not the same as the Pause key.

- 2.0 - Forward
- 2.1 - Rewind
- 2.2 - Pause
- 2.3 - Play
- 2.5 - Forward
- 2.6 - Rewind
- 2.7 - Rewind
- 2.8 - Forward
- 2.9 - UNKNOWN
- 2.10 - Next
- 2.11 - Previous

## Set 3 - D-Pad

- 3.0 - Down
- 3.1 - Left
- 3.2 - OK
- 3.7 - Right
- 3.8 - Up

## Set 4 - Nav

- I wasn't able to get much about 4.0, 4.1, 4.3, 4.5, 4.15, or 4.16.
- I have no idea what 4.4 is.w

- 4.0 - Back
- 4.1 - Back
- 4.3 - Home or Exit
- 4.4 - UNKNOWN
- 4.5 - Home or Exit
- 4.6 - Show status bar overlay
- 4.8 - Toggle settings pane
- 4.15 - Home or Exit
- 4.16 - Home or Exit
- 4.17 - Options

## Set 5 - Audio

- 5.0 - Audio -1
- 5.1 - Audio +1
- 5.2 - Toggle mute
- 5.3 - Toggle mute
- 5.4 - Toggle mute

## Set 7 - Input

- 7.1 - Source

## Set 8 - Channel

- 8.0 - Channel down
- 8.1 - Channel up

## Set 11 - Power

- For 11.1 and 11.2, it's recommended to send a WoL packet.

- 11.0 - Power off
- 11.1 - Power on
- 11.2 - Power toggle

## Set 13 - Closed Captions

- 13.0 - Toggle closed captions
- 13.1 - Toggle closed captions
