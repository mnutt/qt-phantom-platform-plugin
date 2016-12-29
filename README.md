# Phantom Qt headless qpa plugin

This is the headless platform plugin for qt, extracted from https://github.com/ariya/phantomjs. It can be used to run Qt applications without an x server.

This plugin will automatically use fontconfig whereas qt's built-in `headless` plugin will not.

## Building

```
qmake
make
```

Copy plugins/platform/libqphantom.so to your qt platform plugin directory, likely `/usr/plugins/platform/`

## Usage

Set the `QT_QPA_PLATFORM=phantom` environment variable before running your application.

## License

See `LICENSE.BSD`
