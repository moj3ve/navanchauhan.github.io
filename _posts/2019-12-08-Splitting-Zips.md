# Splitting ZIPs into Multiple Parts

**Tested on macOS**

Creating the archive:

```
zip -r -s 5 oodlesofnoodles.zip website/
```

5 stands for each split files' size (in mb, kb and gb can also be specified)

For encrypting the zip:

```
zip -er -s 5 oodlesofnoodles.zip website
```

Extracting Files

First we need to collect all parts, then

```
zip -F oodlesofnoodles.zip --out merged.zip
```
