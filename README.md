# ckb-next v0.4.4

## Notes

I did this on a fresh install of macOS Monterey 12.6.3 (21G419), with [Homebrew](https://brew.sh) installed on 23/03/04.

## Install

1: Open term, run:
```
brew install cmake qt5 quazip
echo 'export PATH="/usr/local/opt/qt@5/bin:$PATH"' >> ~/.profile
export LDFLAGS="-L/usr/local/opt/qt@5/lib"
export CPPFLAGS="-I/usr/local/opt/qt@5/include"
```

2: Download [ckb-next-v0.4.4](https://github.com/anizee/ckb-next-v0.4.4/raw/main/ckb-next_v0.4.4.dmg), and install

3: Restart computer in recovery and run:
```
csrutil disable
spctl kext-consent add G43BCU2T37
```

4: Reboot to macOS, open term and run:
```
sudo kextload "/Library/Extensions/org.pqrs.driver.Karabiner.VirtualHIDDevice.v060800.kext"
```

5: Add daemon to Input Sources:
```
/Library/Application\ Support/ckb-next-daemon
```

5: Restart computer in recovery and run:
```
csrutil enable
```
