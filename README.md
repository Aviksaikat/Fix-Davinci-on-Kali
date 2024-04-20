# Fix-Davinci-on-Kali
Fix to run Davinci Resolve on Kali &amp; Debian based distros

## Error
```sh
undefined symbol: g_string_free_and_steal
```

## Fix 
Search for the missing libraries and install them from sources. In my case `libgdk_pixbuf-2.0.so.0` & `libpango-1.0.so.0` were missing so I installed them from Debian sources & after that, Davinci ran smoothly. I'm adding the latest versions(at the time of creating this repo) of those in this repo.

- [libgdk_pixbuf-2.0.so.0](http://ftp.mx.debian.org/debian/pool/main/g/gdk-pixbuf/libgdk-pixbuf-2.0-0_2.42.10+dfsg-1+b1_amd64.deb)
- [libpango-1.0.so.0](http://ftp.us.debian.org/debian/pool/main/p/pango1.0/libpango-1.0-0_1.50.12+ds-1_amd64.deb)

## Nvidia GPU not detected by Davinci
Follow the steps mentioned [here](https://github.com/Aviksaikat/Hashcat-GPU-fix-for-kali)



**N.B.** I was able to solve my issue by following these steps it may not be the case for you :).
