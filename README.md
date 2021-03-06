# PandasGui

A GUI for analyzing Pandas DataFrames.

<img src="https://imgur.com/LEAQfa1.gif" alt="Demo" width="750"/>

## Installation

Install latest release from PyPi:

```shell
pip install pandasgui
```

Install directly from Github for the latest unreleased changes:

```shell
pip install git+https://github.com/adamerose/pandasgui.git
```

## Usage

Create and view a simple DataFrame

```python
import pandas as pd
from pandasgui import show

df = pd.DataFrame(([[1, 2, 3], [4, 5, 6], [7, 8, 9]]), columns=['a', 'b', 'c'])
show(df)
```

Or if you are running your code as a script instead of in IPython, you will need to block execution until you close the GUI

```python
show(df, settings={'block': True})
```

PandasGUI comes with sample datasets that will download on first use. You can also import `all_datasets` which is a dictionary of all the sample datasets

```python
from pandasgui import show
from pandasgui.datasets import pokemon, titanic, all_datasets
show(pokemon, titanic)
show(**all_datasets)
```

## Features

- View DataFrames and Series (with MultiIndex support)
- Interactive plotting
- Filtering
- Statistics summary
- Data editing and copy / paste
- Import CSV files with drag & drop
- Search toolbar

## More Info

This project is still in version 0.x.y and subject to breaking changes. Latest changes will be on the `develop` branch, and will be occasionally merged to `master` as a release with a tag indicating the version number, and published to PyPi.

Issues, feedback and pull requests are welcome.

Remember to leave a ⭐ if you like this!

## Screenshots

DataFrame Viewer

<img src="https://imgur.com/hUnuBiY.png" alt="Screenshot" width="500"/>

Filters

<img src="https://imgur.com/Yn0Zqa6.png" alt="Screenshot" width="500"/>

Statistics

<img src="https://imgur.com/mKCaaNM.png" alt="Screenshot" width="500"/>

Grapher

<img src="https://imgur.com/zZIeAzj.png" alt="Screenshot" width="500"/>

MultiIndex Support

<img src="https://imgur.com/2rz9OzC.png" alt="Screenshot" width="500"/>
