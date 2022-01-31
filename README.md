# far2l-macros

A collection of keyboard macros for Linux port of FAR v2: https://github.com/elfmz/far2l

This is useful for example if you use a MacBookPro 13" keyboard, which doesn't have keys such as ```Ins```.

--

Create the directory ```~/.config/far2l/REG/HKU/c/k-Software/k-Far2/k-KeyMacros``` and a subdirectory named according to the part of UI where the keyboard macro should work. For dialogs, e.g. ```Commands->File Associations``` the subdirectory must be named ```k-Menu```. 

Each macro consists of a subdirectory named by the actual key combination on your keyboard, containing files specifying the target combination to be emulated, effective after you restart ```far2l```.

**Example:** to emulate ```Ins``` using ```Ctrl+I``` in menus/dialogs you might create a directory

```~/.config/far2l/REG/HKU/c/k-Software/k-Far2/k-KeyMacros/k-Menu/k-CtrlI``` 

and create a file in there named ```v-Sequence``` containing:
```
Sequence
SZ
Ins\0
```

Jan 2022 update: in newer far2l's versions key macros are stored differently. Put key_macros.ini into ```~/.config/far2l/settings```
