## waf-gtkbuilder

A simple unit for automatically checking GtkBuilder/Glade xml files for validity.

### Usage

Just copy the `gtkbuilder.py` file to your project directory (where the desired waf file is, other wise you have to adjust the `tooldir=` path)

```python
def options(opt):
    ...

def configure(cfg):
    ...


def build(bld):
	bld.load('gtkbuilder', tooldir='.')

	bld(source='gtkbuilder.ui tool.ui verify.ui please.ui')

```
