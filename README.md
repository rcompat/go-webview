# gio plugins

Get a webview and Deep Link working

https://github.com/rcompat/rcompat/issues/25#issuecomment-2220450531

Here is my basic approach to get working quickly:

1. Use a Makefile so that me and others can dive in and help. You need the right version of GIO and gio cmd setup. I have some makefiles for this.

2. Get the cross compile tool chain going for Mobile and Desktop such that end devs can also do it. 
- Modify https://github.com/gedw99/goup to work with GIO.

3. Test on Web, Desktop and Mobie
- Browserstack has real hardware for Web and Mobile Testing.
- https://www.browserstack.com/

4. Explore the wrapping or it for Primate.



