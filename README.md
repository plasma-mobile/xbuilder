Welcome to the wonderful world of cross compilation. Where magic is possible and things break unexpectedly!

What we're going to do here is to create a debian&ubuntu-based system with armhf cross-compilation capabilities. Since we won't be able to properly access the whole system, it mounts a suggested directory so that you can access the source-code for building purposes.

To get get started we'll do the following:

```
sudo ./setup.sh <your projects path>
```

This will take a while. You can grab a cup of $YOUR_FAVORITE_DRINK.

Once it's ready, you'll get a "go-mobile" executable that will let you in the system, you just need to execute it.

``` ./go-mobile ```

That should give you a workable environment.

Check xutils repository to see some extra available tools inside

While configuring a project with cmake, is important to add
the following in order to cmake to work a second time
-DCMAKE_TOOLCHAIN_FILE=/usr/share/cmake-3.0/Modules/MultiArchCross.cmake
