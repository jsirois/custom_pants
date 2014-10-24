This repo serves as a demonstration of building a custom multiplatfrom pants pex.

To test things out:
```console
$ ./pants goal binary //:pants
```

And to verify the produced pex for the current platform, it can be dogfooded against itself:
```console
$ ./dist/pants.pex goal binary //:pants
```
