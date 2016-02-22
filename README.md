# xrff2csv

A Python tool that converts XRFF files to CSV format.

## License

Please see the [repository license](https://github.com/rhiever/xrff2csv/blob/master/LICENSE) for the licensing and usage information for xrff2csv.

Generally, we have licensed xrff2csv to make it as widely usable as possible.

## Installation

```bash
pip install xrff2csv
```

## Usage

xrff2csv can be used on the command line. Use `--help` to see its usage instructions.

```bash
xrff2csv --help

usage: xrff2csv [-h] [-i INPUT_FILENAME] [-o OUTPUT_FILENAME] [-sep SEP]
                [--version]

A Python tool that converts XRFF files to CSV format.

optional arguments:
  -h, --help          show this help message and exit
  -i INPUT_FILENAME   XRFF file to convert.
  -o OUTPUT_FILENAME  CSV file to output to.
  -sep SEP            Separator in the CSV file (default: \t)
  --version           Display the current xrff2csv version
```

An example use on the command line would be:

```bash
xrff2csv -i zoo.xrff -o zoo.csv -sep ,
```

This command would convert `zoo.xrff` to `zoo.csv` with commas (,) as the separator.

xrff can also be used programmatically. An example use in code would be:

```python
from xrff2csv import xrff2csv

xrff2csv('zoo.xrff', 'zoo.csv', sep=',')
```

## Contributing to xrff2csv

We welcome you to [check the existing issues](https://github.com/rhiever/xrff2csv/issues/) for bugs or enhancements to work on. If you have an idea for an extension to xrff2csv, please [file a new issue](https://github.com/rhiever/xrff2csv/issues/new) so we can discuss it.
