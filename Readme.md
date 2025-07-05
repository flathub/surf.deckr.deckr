### Deckr app

For more information: [deckr.surf](https://deckr.surf)

[flathub listing](https://github.com/flathub/surf.deckr.deckr)

[Maintainance documentation](https://github.com/flathub/flathub/wiki/App-Maintenance)

flatpak run --verbose surf.deckr.deckr

appstreamcli validate --explain surf.deckr.deckr.metainfo.xml

git submodule init
git submodule update
git submodule update --init --recursive

build-options:
env:
PKG_CONFIG_PATH: /app/lib/pkgconfig:/app/share/pkgconfig:/app/lib64/pkgconfig
