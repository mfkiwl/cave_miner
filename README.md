# ℂᎪᏙᎬ || ᎷⅠℕᎬᎡ
This tools search for code cave in binaries (Elf, Mach-o, Pe)

### Installation

```bash
pip install cave-miner
```

### Usage

```
❯ cave_miner --help
    /========\
   /    ||    \
        ||
        ||
        ||
   ℂᎪᏙᎬ || ᎷⅠℕᎬᎡ

Search for code cave in all binaries
Usage:
  cave_miner search [--size=<size>] <file_name>

Options:
  -h --help      Show this help
  --version      Show the program version
  --size=<size>  The minimum size of the cave in bytes [default: 256]
```

### Exemple

```
❯ cave_miner search ~/Downloads/putty.exe                                                                      cave_miner/git/master

    /========\
   /    ||    \
        ||
        ||
        ||
   ℂᎪᏙᎬ || ᎷⅠℕᎬᎡ

[*] Starting cave mining process...

[*] New cave detected !
  section_name: .rdata
  cave_begin:   0x0009a314
  cave_end:     0x0009a418
  cave_size:    0x00000104

[*] New cave detected !
  section_name: .rdata
  cave_begin:   0x0009a517
  cave_end:     0x0009a618
  cave_size:    0x00000101

[*] New cave detected !
  section_name: .data
  cave_begin:   0x000a0ae5
  cave_end:     0x000a0c3c
  cave_size:    0x00000157

[*] Mining finished.
```