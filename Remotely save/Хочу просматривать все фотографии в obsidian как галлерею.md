---
Ddd: Dd
Test: [test]
---

И оперировать фотографиями как в галерее

``` note-gallery
sort: desc
limit: 100
breakpoints: 1
```


``` g img-gallery
path: /
type: vertical
mobile: 4
```



``` page-gallery
# Any options given at the root level of the configuration
# will be used as defaults for all views (but can be overridden
# in any individual view).
fields: [file.name]
columns: 3
orientation: landscape

# If you don't include an explicit `views` option (which needs
# to be an array), then page-gallery will just use all the root
# level options as a single unnamed view.
views:
  - name: Yosemite
    from: '"/" AND #yosemite'
  - name: Yellowstone
    from: '"Images" AND #yellowstone'
    columns: 4
    orientation: portrait
```

```page-gallery
title: gg
views:
  - name: Yosemite
    from: 
    columns: 1
    orientation: portrait
```