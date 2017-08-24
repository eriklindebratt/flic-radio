# flic-radio

> Internet radio controlled using the Flic button. Suitable to run on e.g. a Raspberry Pi.

## Setup

Download the [Flic Linux SDK](https://github.com/50ButtonsEach/fliclib-linux-hci) and place it in the directory as the `flic-client` script.

The script assumes you have the `mplayer` package installed on your system; if not, install it.

Configure your ratio stations in by modifying the `audioStreams` variable in the `flic-client` script. Default stations are P1, P2 and P2 from the Swedish national radio broadcaster [Sveriges Radio](https://sverigesradio.se/).

## Optional

Configure [supervisord](http://supervisord.org/) to start the Flic server (bundled as part of the Flic Linux SDK) and the `flic-client` script on boot.

`supervisord-reference-configs/flic-server` and
`supervisord-reference-configs/flic-client` can be used as a reference to configure supervisord. Please refer to [supervisord's own documentation](http://supervisord.org/running.html#adding-a-program) for further details on how to add a program.

## Usage

- Press Flic button once to toggle the radio playback.
- Double press the Flic button to switch radio station.
- Press and hold down the Flic button to reboot the whole computer 😱.
