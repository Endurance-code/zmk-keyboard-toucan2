# ZMK config for beekeeb Toucan2 Keyboard

[The beekeeb Toucan2 Keyboard](https://beekeeb.com/introducing-toucan2/) is a wireless split 42-key column‑stagger keyboard that a display and a trackpad, with an aggressive stagger on the pinky columns.

# Customizations

- **Keymap**: [config/toucan.keymap](config/toucan.keymap)
- **General configs**: [boards/shields/toucan/toucan_left.conf](boards/shields/toucan/toucan_left.conf) and [boards/shields/toucan/toucan_right.conf](boards/shields/toucan/toucan_right.conf)
- **Swipe shortcuts**: the `swipe_button_mapper` node in [boards/shields/toucan/toucan.dtsi](boards/shields/toucan/toucan.dtsi)
- **Invert scroll / trackpad settings**: the `tps43_trackpad` node in [boards/shields/toucan/toucan_right.overlay](boards/shields/toucan/toucan_right.overlay)

# custom key config

I fork the original Toucan2 github repo to my own account to customize.
I use https://nickcoutsos.github.io/keymap-editor/ for the keymap editor, its a super fast way to edit behaviors and keymapping.
I like auto shift so, I make a new behavior and title it 'AS', I like 300ms for the hold function to work.
Then I like QWERTY, so I change each key from 'KP' to 'AS', with the hold key as LSHIFT and the letter, and the tap being just the letter.
When done, save in the keymap editor to commit.

After customization, the Trackpad commands can be commented out or left in for your desired config.

Lastly, go to github actions, and download the last runtime's firmware at the bottom, plug in toucan, if Seed, double press the button after plug in and can access its file. Drag in the Left or Right file to the appropriate keyboard, after its done and shutsoff, the keyboard is ready for use, 

# License

The code in this repo is available under the MIT license.

The included shield nice_view_gem is modified from https://github.com/M165437/nice-view-gem licensed under the MIT License.

The linked trackpad module is based on https://github.com/geeksville/zmk_driver_azoteq

ZMK code snippets are taken from the ZMK documentation under the MIT license.

The embedded font QuinqueFive is designed by GGBotNet, licensed under under the SIL Open Font License, Version 1.1.
