# Less common stuff to do with the command prompt

## Unmount drive using the command line

```bat
diskpart

::list volumes
list volume

::assuming that the volume of the removable drive is number 4
select volume 4

::now unmount disk
remove all dismount

::we can see the unmounted volume by listing the volumes again (the volume should be shown to be offline)
list volume
```

## View current Windows product key from the command line

```bat
:: the following returns the product key
wmic path softwarelicensingservice get OA3xOriginalProductKey
```
