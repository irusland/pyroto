# autoproto

`autoproto` is a Python project designed to generate source files from Protocol Buffers (protos) using the `PackageGenerator` class.

##

```python
import logging
from pathlib import Path

from protopy import PackageGenerator

logging.basicConfig(level=logging.DEBUG)


if __name__ == '__main__':
    generator = PackageGenerator()
    base_dir = Path().parent.absolute() / 'usage'

    generator.generate_sources(
        proto_dir=base_dir / 'protos',
        out_dir=base_dir / 'package',
    )

```

## Features

- Generates source files from Protocol Buffers.
- Packages the generated sources for easy usage.

```sh
pip install protopy

```

## Development
### Installation

