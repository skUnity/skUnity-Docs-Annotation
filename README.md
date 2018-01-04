# skUnity-Docs-Annotation
The official annotation used to import syntax to the docs.


# Adding to your Addon
To add this to your addon, you have to copy the SKU class into your plugin and change the package to one of your own.


# How to use
These annotations work best with syntax loaded staticly with Skript's native registration system. Here is an example:
```java
@SKU.data(
        name = "Name of the Element",
        desc = "Description of the element.",
        example = "An example "
)
public class SampleEffect extends Effect {

    static {
        Skript.registerEffect(SampleEffect.class, "[syn]tax");
    }
```
