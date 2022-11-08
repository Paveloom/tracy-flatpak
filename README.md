### Description

This repository provides a Flatpak manifest for the [Tracy Profiler](https://github.com/wolfpld/tracy).

#### Git mirrors
- [Codeberg](https://codeberg.org/paveloom-a/Tracy)
- [GitHub](https://github.com/paveloom-a/Tracy)
- [GitLab](https://gitlab.com/paveloom-g/apps/tracy)

#### Build

Make sure you have installed
- [`flatpak-builder`](https://github.com/flatpak/flatpak-builder);
- `org.freedesktop.Platform//22.08` and `org.freedesktop.Sdk//22.08`.

Then, run

```
flatpak-builder --user --install --force-clean build manifest.yml
```

If the build is successful, you will now be able to run the Flatpak as usual:

```
flatpak run tracy.profiler.Tracy
```

You might also want to delete the `build` and `.flatpak-builder` directories after you're done.
