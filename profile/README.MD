Document language based on [SDLang](https://sdlang.org) and [KDL](https://kdl.dev) with Game Development in focus

```c
abstract:item type="item" {
    size 0.2 1 3
    model "madel/cube.obj"
    texture "texture/missing.png"
    material "material/missing.mtl"
    pointlessProp "i am prop"
    transform {
        1 0 0 0
        0 1 0 0
        0 0 1 0
        0 0 0 1
    }
    glow on
}

override abstract:item {
    override model "model/cube.obj"
}

override abstract:item {
    delete pointlessProp
}

armor inherit=abstract:item type="pickup" interactable
```
