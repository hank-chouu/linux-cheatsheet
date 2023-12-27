# Linux Cheatsheet

The resources are mostly for Arch-Linux based distos.

**Connect iPhone to Linux**

https://itsfoss.com/iphone-antergos-linux/

**Convert HEIC in Linux**

https://www.baeldung.com/linux/view-heic-images

**Add extension to gsettings schemas**

```
mkdir -p .local/share/glib-2.0/schemas
cp .local/share/gnome-shell/extensions/{UUID}/schemas/org.gnome.shell.extensions.{NAME}.gschema.xml .local/share/glib-2.0/schemas/
cd .local/share/glib-2.0/schemas/
glib-compile-schemas .
cd
gsettings list-recursively org.gnome.shell.extensions.{NAME}
```