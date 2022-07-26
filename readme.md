# Less common stuff to do with the command prompt

## Dismount drive using the command line

```bat
diskpart

::list volumes
list volume

::assuming that the volume of the removable drive is number 4
select volume 4

remove all dismount
```
