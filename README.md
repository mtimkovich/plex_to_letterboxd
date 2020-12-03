# Plex2Letterboxd

Exports watched movies from Plex to the [Letterboxd Import Format][import].

Movies are exported to a CSV file containing:
* Movie Title
* Release Year
* User Rating
* Last Watched Date

## Installation

```
$ git clone https://github.com/mtimkovich/plex2letterboxd.git
$ cd plex2letterbox
$ pip install .
```

## Usage

Rename `config.ini.example` to `config.ini` and fill it with your Plex credentials.

```
$ python -m plex2letterboxd -i config.ini
```

```
optional arguments:
  -h, --help            show this help message and exit
  -i INI, --ini INI     config file
  -o OUTPUT, --output OUTPUT
                        file to output to
```

The generated CSV file can be uploaded to Letterboxd at https://letterboxd.com/import/.

## Author

[Max Timkovich][profile]

[import]: https://letterboxd.com/about/importing-data/
[profile]: https://letterboxd.com/djswerve/
