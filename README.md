# SX1509 GPIO Expander Package

This package provides a Python interface for controlling the SX1509 GPIO expander.

## Installation

Install the package using pip:

```python
pip install sx1509-gpio-expander
```

## Usage

```python
from sx1509_gpio_expander import SX1509
import board

# Configure I2C
i2c = board.I2C() 
# Create an instance of the SX1509
ioExpander = SX1509.SX1509(i2c, 0x3E)

# Now you can use the expander
ioExpander.pinMode(0, ioExpander.OUTPUT)
ioExpander.digitalWrite(0, ioExpander.HIGH)
```

## License

This project is licensed under the GNU GENERAL PUBLIC LICENSE - see the [LICENSE](LICENSE) file for details.
