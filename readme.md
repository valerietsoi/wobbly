|||
|---|---|
| ![image](images/IMG_5291.png) | ![image](images/IMG_5292.png)|


[toc]


## firmware

### method

<b>Step 1</b>
Clone [vial](https://get.vial.today/docs/porting-to-vial.html) to local device and place `firmware` folder into `vial/keyboards`

<b>Step 2</b>
Terminal: `cd` to vial (where keyboard, lib, layouts directories are).

<b>Step 3</b> 
Run 
```
make <relative_firmware_path>:vial
```
A `<xxx>_vial.uf2` file will then appear in the vial directory.

<b>Step 4</b> 
Open up the case enclosure (1.6mm allen key). Plug microcontroller into device and enter DFU mode by:
 - Hold down BOOT (on rp2040 zero)
 - Click RESET
 - Release BOOT

A new USB device should then appear on your device. Move the `.uf2` into the USB device. 

Now you can remap macros using the [vial web configurator](https://get.vial.today/) 

### more info
Board currently has macros, combos, and tap dance enabled. 

For more information on configuring keymaps/macros and enabling/disabling features (instead of using the vial configurator GUI), see [QMK documention](https://docs.qmk.fm/keymap)

<br>
<br>


## build guide

### bom
| material | quantity | 
|---|---|
| rp2040 zero | 1 |
| awg 26 solid core wire | some |  
| m2 x 3 mm x OD 3.5 heat set inserts | 6 |
| m2 x 8 mm hex bolt | 6 | 
| top case | 1 | 
| bottom case | 1 |
| mechanical switch | 4 | 
| 1N4148 diodes | 4 |  
| 2u keycaps | 4 | 
| plate mounted stabilisers (optional) | 4 | 
| heat shrink tubing (optional) | some | 

<br>

### tools

|tools| 
|---|
| soldering iron |
| allen key 1.6mm |
| wire strippers |
| usb-c to a or c-c data cable |



<br>

### method

1. install heat set inserts 
2. (optional) install stab (+ lube stab before installing, optional)
3. install switches
4. solder wires
5. flash firmware
6. fasten case with screws
7. use

![image](images/IMG_5290.png)

{to be updated}