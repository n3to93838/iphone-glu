## Summary ##

iGLU is an implementation of the
[OpenGL Utility Library](http://www.opengl.org/documentation/specs/)
(GLU) for [iPhone OS](http://developer.apple.com/iphone/).


## License ##

iGLU is based on the GLU source included with
[Mesa](http://mesa3d.sourceforge.net/) 7.2, which in turn derives from
the [SGI OpenGL Sample Implementation](http://oss.sgi.com/projects/ogl-sample/).  All code derived from SGI's source is licensed under
the [SGI Free Software License B](http://oss.sgi.com/projects/FreeB/)
version 2.0. All other code is licensed under the
[MIT license](http://www.opensource.org/licenses/mit-license.php).


## Compiling ##

To compile for the simulator:
```
make ARCH=i386 PLATFORM=iPhoneSimulator
```

To compile for a device:
```
make ARCH=armv6 PLATFORM=iPhoneOS
```

This produces `libGLU.a`, which you can add to your iPhone project
(along with `include/glu.h`).


## Comparison with Standard GLU ##

iGLU does not include GLU features that depend on OpenGL functionality
missing in [OpenGL ES 1.1](http://www.khronos.org/opengles/1_X/).

Available features:

  * Matrix manipulation
  * Polygon tessellation

Missing features:

  * Mipmapping
  * Quadrics
  * NURBS

For more information on these features, see the
[GLU 1.3 specification](http://opengl.org/documentation/specs/glu/glu1_3.pdf).