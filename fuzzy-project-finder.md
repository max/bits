If you have a projects folder with all your source code install selecta and use this simple bashscript to trigger a fuzzy finder:

```bash
proj() {
  cd $(find ~/Projects -maxdepth 1 -type d | selecta)
}
```

You can install `selecta` with homebrew:

```
brew install selecta
```
