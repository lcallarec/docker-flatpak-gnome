# flatpak-gnome

Ubuntu based-image that contains flatpak and __gnome__ remote repository.

You'll just have to use this images as base for your own-backed __Dockerfile__.

This images was designed for continuous integration on TravisCI, where the only way to run flatpak is inside a docker container.

It doesn't came with provisionned Runtimes nor Sdk to limit the images size, so you sstill have to install the ones you need :

```bash
docker exec -ti flatpak-gnome flatpak
```
