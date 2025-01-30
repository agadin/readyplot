#!/usr/bin/env python3
# -*- coding: utf-8 -*-
"""
Created on Wed Jan 29 11:26:49 2025

@author: paveyboys
"""

# My Plotting Package

A class-based plotting package with defaults that easily provide scientific
publication-ready plots in the style of popular graphing software. Perfect
for automatically creating many plots at once that are all ready to use.

## Installation

You can install the package via pip:

```bash
pip install readyplot
````
## Usage
```{python}
from readyplot.scatter_plotter import ScatterPlotter
plotter = ScatterPlotter('box_strip',DF,MechVars[1],Var,'Surgery',colors=['c','m','g'],
                                dodge=True,folder_name = folder_name,low_cap0=True,
                                handles_in_legend = 3,fig_width = 10,box_width = 0.9,
                                custom_y_label =Var + ' (' + Units[MechVars.index(Var)]+')')  
plotter.large_loop()
````

### Key Design Considerations:
- **Modularity**: Each plot type (`ScatterPlotter`, `LinePlotter`) is its own class that inherits from a shared `BasePlotter`, making it easy to extend in the future with other types of plots.
- **Customization**: Users can easily customize plot styles, colors, labels, etc., through constructor parameters.
- **Testability**: The package includes unit tests to verify the functionality of different components.
- **Documentation**: The `README.md` provides clear usage examples and installation instructions.

---

### Conclusion
This template sets up a simple, maintainable structure for a class-based plotting package. You can easily expand on this by adding more plot types, enhancing the base class with more reusable functionality, or adding more utilities. It adheres to common Python conventions, and with a proper test suite, it will be easy to keep track of changes and bugs.

Let me know if you need more details or help with specific aspects of this!
                                