### Description

This repository provides a Flatpak manifest for the [Tracy Profiler](https://github.com/wolfpld/tracy).

The source is the latest commit from the `master` branch.

#### Git mirrors
- [Codeberg](https://codeberg.org/paveloom-a/Tracy)
- [GitHub](https://github.com/paveloom-a/Tracy)
- [GitLab](https://gitlab.com/paveloom-g/apps/tracy)

#### Build

Make sure you have installed [`flatpak-builder`](https://github.com/flatpak/flatpak-builder) and [set up](https://flatpak.org/setup) Flatpak with the Flathub remote.

Run

```
flatpak-builder --install-deps-only --install-deps-from=flathub build manifest.yml
```

to check if the dependencies are installed. Then, build with


```
flatpak-builder --user --install --force-clean build manifest.yml
```

If the build is successful, you will now be able to run the Flatpak as usual:

```
flatpak run tracy.profiler.Tracy
```

You might also want to delete the `build` and `.flatpak-builder` directories after you're done.
