# gio plugins

Get a webview and Deep Link working

https://github.com/rcompat/rcompat/issues/25#issuecomment-2220450531

Here is my basic approach to get working quickly:

Make a new repo just for this.

Use a Makefile so that me and others can dive in and help. You need the right version of GIO and gio cmd setup. I have some makefiles for this.

Get the cross compile tool chain going for Mobile and Desktop such that end devs can also do it. So many times with Mobile you have the problem of the other dev having android SDK setup differently etc etc. Thats why I am adapting this https://github.com/gedw99/goup to work with GIO.

Then explore the wrapping or it for Primate. I would NOT try to do anything too complex because getting that code working was a feat in itself IMHO. I would chicken out ( for now ) and just wrap calling the binary for now. I would not do any FFI yet. Now you have a working system at least that I think Primate can use.

Having gotten that far, then I might "chicken in", and try the more fancy approach of the CGO code like the example with oven-sh/bun#369

