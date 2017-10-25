# Failed to load interface for 'Data.Hashable.Generic'

```sh
cabal sandbox init
cabal install --only-dependencies && cabal new-build
cabal install
```

causes an error:

```
Resolving dependencies...
In order, the following will be installed:
failed-to-load-interface-0.1.0.0 (reinstall) (changes: hashable-1.2.6.1 added,
lens-4.15.4 removed)
Warning: Note that reinstalls are always dangerous. Continuing anyway...
Notice: installing into a sandbox located at
/home/ioijoi/program/failed-to-load-interface/.cabal-sandbox
Configuring failed-to-load-interface-0.1.0.0...
Building failed-to-load-interface-0.1.0.0...
Failed to install failed-to-load-interface-0.1.0.0
Build log ( /home/ioijoi/program/failed-to-load-interface/.cabal-sandbox/logs/ghc-8.2.1/failed-to-load-interface-0.1.0.0-60zLfq7fTAM3ByiuYQC8GJ.log ):
cabal: Entering directory '.'
Configuring failed-to-load-interface-0.1.0.0...
Preprocessing library for failed-to-load-interface-0.1.0.0..
Building library instantiated with Foo = <Foo>
for failed-to-load-interface-0.1.0.0..
Installing library in /home/ioijoi/program/failed-to-load-interface/.cabal-sandbox/lib/x86_64-linux-ghc-8.2.1/failed-to-load-interface-0.1.0.0-60zLfq7fTAM3ByiuYQC8GJ
cabal: '/home/ioijoi/.stack/programs/x86_64-linux/ghc-8.2.1/bin/ghc' exited
with an error:
Failed to load interface for ‘Data.Hashable.Generic’
no unit id matching ‘hashable-1.2.6.1-14fEJP30YhAG9w115PODz0’ was found
cabal: Leaving directory '.'
cabal: Error: some packages failed to install:
failed-to-load-interface-0.1.0.0-60zLfq7fTAM3ByiuYQC8GJ failed during the
final install step. The exception was:
ExitFailure 1
```


