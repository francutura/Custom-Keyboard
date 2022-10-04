# Custom-Keyboard
My custom keyboard layout


## Install instructions

### Step 1
```
cp custom_layout /usr/share/X11/xkb/symbols
```
---

### Step 2
> In **/usr/share/X11/xkb/rules** Open files **base.lst** and **evdev.lst**

> In both files Find **! layout** line and insert your own layout definition e.g. below

```
  custom_layout             Main Custom Keyboard
```
---
### Step 3 
> In **evdev.xml**

> Find **\<layoutList\>** line and insert your own layout definition. e.g. below

```
<layout>
    <configItem>
        <name>custom_layout</name>
        <shortDescription>custom_layout</shortDescription>
        <description>Main Custom Keyboard</description>
        <languageList>
            <iso639Id>hrv</iso639Id>
        </languageList>
    </configItem>
</layout>
```