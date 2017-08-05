Icon
====

###### How to compile

- First compile the resource file.

```
cd resources
rc.exe /V resource.rc
cd ..
```

- Now compile the program with resource file.

```
cl.exe /EHsc /DUNICODE /Zi icon.cpp /link resources\resource.res user32.lib kernel32.lib gdi32.lib
```

###### Preview

![icon](preview/icon.png?raw=true "Icon")