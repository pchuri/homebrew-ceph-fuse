# homebrew-ceph-fuse

Ref from https://github.com/mulbc/homebrew-ceph-client. Nautilus support was added.

```
brew install cask osxfuse
brew tap pchuri/homebrew-ceph-fuse
brew install ceph-fuse
```

**Note**

Please refer to link below, When you encounter a error related to python@2. 
https://github.com/pchuri/homebrew-python2


If you have previously installed `mulbc/homebrew-ceph-client`, please:
```
brew remove ceph-client
brew untap zeichenanonym/ceph-client
```
