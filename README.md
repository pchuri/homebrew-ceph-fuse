# homebrew-ceph-fuse

Ref from https://github.com/mulbc/homebrew-ceph-client. Nautilus support was added.

## Intel mac
```
brew install snappy ccache cmake pkg-config cython
brew tap pchuri/homebrew-python2
brew install python@2
 
brew install cask osxfuse
brew tap pchuri/homebrew-ceph-fuse
brew install ceph-fuse
```

## Apple Silicon Mac
Install macFuse from https://osxfuse.github.io
```
arch -x86_64 /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
arch -x86_64 /usr/local/bin/brew install snappy ccache cmake pkg-config cython
arch -x86_64 /usr/local/bin/brew tap pchuri/homebrew-python2
arch -x86_64 /usr/local/bin/brew install python@2
arch -x86_64 /usr/local/bin/brew tap pchuri/homebrew-ceph-fuse
arch -x86_64 /usr/local/bin/brew install ceph-fuse
```

# Troubleshooting
## Error related to python@2
- Please refer to link below
- https://github.com/pchuri/homebrew-python2

## Permission 
- If there is a permission problem during the mount process, please refer to the link below to configure.
- Select the “Allow user management of kernel extensions from identified developers” checkbox to allow installation of software that uses legacy kernel extensions.
- https://support.apple.com/guide/mac-help/macos-recovery-a-mac-apple-silicon-mchl82829c17/11.0/mac/11.0#mchl9b13cbdc
 
# Etc
If you have previously installed `mulbc/homebrew-ceph-client`, please:
```
brew remove ceph-client
brew untap zeichenanonym/ceph-client
```
