# Linux ISO locales

A collection of opinionated locales, using as many ISO standards as possible.

## Installation

### Debian

```bash
git clone https://github.com/gilex-dev/linux-iso-locales
cd linux-iso-locales
sudo cp en_DE_ISO.UTF-8 /usr/share/i18n/locales/
sudo sh -c 'echo "en_DE_ISO.UTF-8 UTF-8" >> /etc/locale.gen'
sudo sh -c 'echo "en_DE_ISO.UTF-8" >> /etc/default/locale.conf'
```

## Contributing

Contributions are welcome.

If you want to contribute, either by adding new or fixing existing locales, create a pull-request I will review it.

## License

[GNU LGPLv2.1](./COPYING.md)
