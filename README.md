AviSynth system build for Sublime Text 3
========================================
This is a basic [ST3 build system][] that runs your `.avs` script externally in [MPC-HC][], my Windows video player of choice.

This is the entire code:

```json
{
    "cmd": ["C:\\Program Files\\MPC-HC\\mpc-hc64.exe", "$file"],
    "file_regex": "avs$",
    "selector": "source.avs",
    "shell": true
}
```

Replace `C:\\Program Files\\MPC-HC\\mpc-hc64.exe` with the path of your preferred video player to use that instead.

Installation
------------
Either:

* copy `AviSynth.sublime-build` to `%APPDATA%\Sublime Text 3\Packages\User`, or
* in ST3, go to **Tools** > **Build System** > **New Build System**, and copy-paste the contents of `AviSynth.sublime-build`

Related projects
----------------
* [avisynth-syntax][] ([memory leak][])


[st3 build system]: https://www.sublimetext.com/docs/3/build_systems.html
[mpc-hc]: https://mpc-hc.org/
[avisynth-syntax]: https://github.com/ndarville/avisynth-syntax
[memory leak]: https://github.com/ndarville/avisynth-syntax/issues/1
