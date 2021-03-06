Nginx + Pagespeed
=================

An nginx container mimicking the [official nginx box](https://registry.hub.docker.com/_/nginx/), but instead using a rebuilt version of the .deb with the [PageSpeed module](https://developers.google.com/speed/pagespeed/module) compiled in.

Versions
--------

-	**Nginx**: 1.17.9-1~stretch
-	**NPS**: 1.13.35.2

Building the .deb package
-------------------------

If you want to rebuild the package files:

```
% docker-compose -f docker-build.yml build
% docker-compose -f docker-build.yml run build
```

Then, the new packages should be in `/packages` folder.
