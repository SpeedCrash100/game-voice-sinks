# Game and Voice Audio mixing

Utils and configuration for mixing Game audio and Voice audio and controlling the volume of each with single value.
See [ChatMix from SteelSeries](https://support.steelseries.com/hc/en-us/articles/360051003931-What-is-ChatMix)

## How to use it?

### Pipewire

1. Edit [./pipewire/10-game-voice-sink.conf] and select target device for output
2. Place the file in ~/.config/pipewire/pipewire.conf.d/
3. Restart pipewire (`systemctl --user restart pipewire`)
4. use [./pipewire/set_chatmix] to set ratio [-1.0 1.0]
