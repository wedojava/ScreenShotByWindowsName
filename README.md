# ScreenShotByWindowsName
ScreenShot implement by C/C++ via VC 6.0

It will capture screen while target windows name exist.

It will get all windows names every 2 second.

In default, only one param follow the command, it can capture 200 pictures then exit.

While capture successfuly, at the same path a folder named `ScrS` can be create and some pictures saved.

Pictures' name is the keyword/param you set,like Chrome1.jpg, Chrome2.jpg...

The sister repository is https://github.com/wedojava/ScreenShotByProcessName

## Why VC6.0

Also, I consider windows XP SP3 can run it well, sometimes, program via VC6.0 can achive my goal.

## Passed test platform

- Windows XP SP3
- Windows 7
- Windows 10

## Usage

    ScreenShotByWindowsName.exe <keyword> [<capture number>]

- `<keyword>`: Your target window name's keyword, Case Sensitively.
- `[<capture number>]`: optional param, how many pictures you want capture, default setting is 200

eg:

- Capture 10 pictures if there is/are process name(s) cantain "Chrome"
```
ScreenShotByWindowsName.exe Chrome 10
```

- Capture pictures 200
```
ScreenShotByWindowsName.exe Chrome
```

## Notice

**It can not identify other language for input param except english.**

It can not return any error at all.

If want to catch the error, just debug source.