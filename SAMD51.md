# Let's port RadioMusic to SAMD51!

This involves altering the firmware a little. It's also reliant on a pair of
library forks, which always makes me uncomfortable.

Once it's running - in my case, off an ItsyBitsy M4 Express, it should be
straightforward to port it to a custom 'rear' board with the same chip, etc, on
it.

## Firmware

* used the [Adafruit Audio library port](https://github.com/adafruit/audio)
* use the stereo output, as Adafruit library doesn't have single output.
* used https://github.com/mitchellpontague/FlashStorage fork of FlashStorage
  with SAMD51 support.
* don't use non-existent analog pins
* update pinouts for ItsyBitsy M4 (TODO update for final)
* TODO: add a USB bootloader

## Hardware

* designed a new back board based around a SAMD51 (not tested yet).

