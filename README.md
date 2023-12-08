# Eyescare

This program will dim the screen for 100 seconds every 30 mins.

Tested on macOS Mojave (10.14), should work on High Sierra (10.13) as well.

## Building

```console
$ pwd
/Users/keepwow/Code/eyescare
% tree
.
├── LICENSE
├── README.md
└── cmd
    └── eyescare
        └── main.go

3 directories, 3 files
$ go build -o ~/bin/eyescare cmd/eyescare/main.go
```

## Usage

### Get current brightness

```console
% eyescare
Usage: eyescare please
This program dims the screen for 100 seconds every 30 minutes.
It only runs when there is exactly one argument named 'please'.
$ eyescare please
2023-12-08 14:21:59: Current brightness is 29.589844
...
```

## Requirement

Make sure the screen saver set to at least every 2 mins.

`Settings -> Battery -> Turn display off after [2:] minutes.`

## Thanks to

- [macos-brightness](https://github.com/mafredri/macos-brightness): Your friendly neighbordhood macOS brightness CLI. Sets the brightness of the builtin display (e.g. on MacBooks).
