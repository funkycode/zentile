<p align="center">
  <img src="/docs/zentile-logo.png" alt="zentile logo"/>
</p>

On-demand tiling for Openbox, Xfce and other [EWMH Complaint Window Managers](https://en.m.wikipedia.org/wiki/Extended_Window_Manager_Hints).

![zentile screencast](docs/screencast.gif)

## FEATURES
- Workspace based tiling. You can enable tiling in one workspace and leave others untouched.
- Comes with two simple tiling layouts (Vertical & Horizontal)
- Customizable gap between tiling windows.
- Autodetection of panels and docks.

## INSTALLATION
**Binary Release**

Download appropriate executable from [releases page](https://github.com/blrsn/zentile/releases)

```
$ chmod a+x zentile-linux-amd64
$ ./zentile-linux-amd64
```

**Go get**

```
$ go get github.com/blrsn/zentile
$ "$GOPATH/bin/zentile"
```

### Commands

Keybinding                                          | Description
----------------------------------------------------|---------------------------------------
<kbd>Ctrl</kbd>+<kbd>Shift</kbd>+<kbd>t</kbd>       | Tile current workspace 
<kbd>Ctrl</kbd>+<kbd>Shift</kbd>+<kbd>u</kbd>       | Untile current workspace
<kbd>Ctrl</kbd>+<kbd>Shift</kbd>+<kbd>s</kbd>       | Cycle through layouts
<kbd>Ctrl</kbd>+<kbd>Shift</kbd>+<kbd>n</kbd>       | Goto next window
<kbd>Ctrl</kbd>+<kbd>Shift</kbd>+<kbd>p</kbd>       | Goto previous window
<kbd>Ctrl</kbd>+<kbd>]</kbd>                        | Increase size of master windows
<kbd>Ctrl</kbd>+<kbd>[</kbd>                        | Decrease size of master windows
<kbd>Ctrl</kbd>+<kbd>Shift</kbd>+<kbd>i</kbd>       | Increment number of master windows
<kbd>Ctrl</kbd>+<kbd>Shift</kbd>+<kbd>d</kbd>       | Decrement number of master windows

The config file is located at `~/.config/zentile/config.toml`

**Note:** Zentile has been tested on Openbox. It should work with any EWMH complaint window manager.

### Credits

Inspired by BurntSushi's [pytyle](https://github.com/BurntSushi/pytyle3).  
This project would not have been possible without [xgbutil](https://github.com/BurntSushi/xgbutil).  
Theme used in the screencast above, comes from addy-dclxvi's [openbox theme collection](https://github.com/addy-dclxvi/openbox-theme-collections).

## License

zentile is licensed under the MIT License. See the full license text in [`LICENSE`](LICENSE).
