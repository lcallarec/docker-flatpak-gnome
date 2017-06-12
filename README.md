# flatpak-gnome

Ubuntu based-image that contains __[flatpak](http://flatpak.org/)__ and __[gnome](http://flatpak.org/runtimes.html)__ remote repository.

You'll just have to use this image as base for your own-backed __Dockerfile__.

This image was designed for _continuous integration_ on __[TravisCI](https://travis-ci.org/)__, where the only way to run __flatpak__ is _inside_ a _docker_ container.

It doesn't came with provisioned Runtimes nor Sdk's to limit the images size, so you still have to install the ones you really need.

For exemple, if you plan to target only Gnome 3.16 & 3.18 runtimes, just run :

```bash
docker pull lcallarec/flatpak-gnome
docker run lcallarec/flatpak-gnome flatpak install gnome org.gnome.Platform//3.16 org.gnome.Platform//3.18
```
