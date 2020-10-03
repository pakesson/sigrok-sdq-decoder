# Note: This has now been merged upstream (commit [b094e81](https://github.com/sigrokproject/libsigrokdecode/commit/b094e81353b3c0c0e9bf5a8ee53bb1da3a05d276))

Sigrok protocol decoder for the SDQ protocol. The SDQ protocol was developed by
Texas Instruments, and is used in devices like the
[bq26100](https://www.ti.com/lit/ds/symlink/bq26100.pdf) battery pack
authentication IC. Apple uses SDQ in devices with MagSafe or Lightning
connectors, as well as in some batteries.

Screenshot from PulseView:
![PulseView screenshot](screenshot.png)

# Installation

The easiest way to use this protocol decoder is to drop it in its own
subdirectory under `~/.local/share/libsigrokdecode/decoders` (Linux) or
`%ProgramData%\libsigrokdecode\decoders` (Windows). Create the directory
if it does not exist.

Example:
```sh
mkdir -p ~/.local/share/libsigrokdecode/decoders
cd ~/.local/share/libsigrokdecode/decoders
git clone https://github.com/pakesson/sigrok-sdq-decoder.git sdq
```

# Example data

An example dump of an iPhone SE being plugged into an untrusted computer can be found under `examples/`.

# Alternatives

If you use Saleae Logic, check out [SDQAnalyzer](https://github.com/nezza/SDQAnalyzer) by Thomas Roth.
