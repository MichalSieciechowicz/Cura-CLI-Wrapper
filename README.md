# Cura CLI Wrapper

This is a small wrapper providing an easy to use CuraEngine:
- alike usage as `slic3r` or `prusa-slicer`
- query hundreds of settings with `cura-slicer` direct with `-h` switch or `--help`

See [Cura CLI Wrapper (cura-slicer)] for details.

# Supported Platforms
- Linux Ubuntu/Debian, tested with Ubuntu 20.04 LTS

# Download
```
% git clone https://github.com/Spiritdude/Cura-CLI-Wrapper
% cd Cura-CLI-Wrapper/
```

# Installation
```
% make requirements
% make install
```

# Usage
```
USAGE Cura-Slicer 0.0.5 aka Cura-CLI-Wrapper (CuraEngine 4.4.1): [<opts>] <file.stl> ...
   options:
      -v or --verbose         increase verbosity
      -vv or --verbose=2          "       "
      --version               display version and exit
      --load=<config>         load config file
      --load <config>           "         "
      --output=<fn>           set output filename
      --output <fn>             "         "
      -o <fn>                   "         "
      --<k>=<v>               set CuraEngine settings (keys with '-' will be converted to '_')
      -h or --help            display all settings
      -h or --help <term> ..  display settings matching term

   examples:
      cura-slicer --help
      cura-slicer --help retract
      cura-slicer -hv retract 
      cura-slicer sphere.stl
      cura-slicer overhang.stl --output=sample.gcode
      cura-slicer overhang.stl --layer-height=0.1 --support-enable=true -o sample.gcode

```

