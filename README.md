pa-volume-monitor
=================

Gives visual feedback with libnotify popups when PulseAudio
volumes are changed. Monitors all sinks and sources, not just
the default one.

For communication with PulseAudio, the PA module
module-dbus-protocol is required. Use `pa-volume-monitor-wrapper`
to load it at runtime or add `load-module module-dbus-protocol`
to `/etc/pulse/default.pa` or `~/.pulse/default.pa`.

## Configuration

See `pa-volume-monitor.cfg`. Configuration file is read from
`/etc/pa-volume-monitor.cfg` and `~/.pa-volume-monitor.cfg`.

## Requirements

- python-notify
- python-dbus
- python-gobject
