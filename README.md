# Linux ISO locales

A collection of opinionated locales, using as many ISO standards as possible.

Inspired by Wilbert van Ham's [ISO Linux](https://www.socsci.ru.nl/wilberth/computer/isoLinux.php).

## Installation

### Debian

```bash
git clone https://github.com/gilex-dev/linux-iso-locales
cd linux-iso-locales
sudo cp en_DE_ISO.UTF-8 /usr/share/i18n/locales/
sudo sh -c 'echo "en_DE_ISO.UTF-8 UTF-8" >> /etc/locale.gen'
sudo locale-gen en_DE_ISO.UTF-8
sudo localectl set-locale LANG=en_DE_ISO.UTF-8
source /etc/locale.conf
```

### Fedora

```bash
sudo dnf install -y glibc-locale-source
git clone https://github.com/gilex-dev/linux-iso-locales
cd linux-iso-locales
sudo cp en_DE_ISO.UTF-8 /usr/share/i18n/locales/
sudo localedef --no-archive --inputfile=en_DE_ISO.UTF-8 --charmap=UTF-8 en_DE_ISO.UTF-8
sudo localectl set-locale LANG=en_DE_ISO.UTF-8
source /etc/locale.conf
```

## Contributing

Contributions are welcome.

If you want to contribute, either by adding new or fixing existing locales, create a pull-request and I will review it.

## License

[GNU LGPLv2.1](./COPYING.md)
