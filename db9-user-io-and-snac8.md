# DB9 User IO and SNAC8

Antonio Villena's DB9 [MiSTer models](https://www.antoniovillena.es/store/product-category/mister/) (SLIM, DRIVE, MINI and PLUS) as well as the [MiSTer Mini-ITX Ironclad Plus](https://www.d3fmod.com/product/mini-itx_ironclad_plus/) have DB9 user IO ports that offer DB9 and SNAC8 functionality.

## Table of Contents

* [Summary](#summary)
* [DB9/SNAC8 Forks with ENCC](#db9-snac8-forks-with-encc)
* [DB9 User IO](#db9-user-io)
* [SNAC8](#snac8)

## Summary

The DB9 and SNAC8 forks with Extended Native Controller Compatibility allow you to do the following:

* Control the main MiSTer menu, as well as the menus and games for compatible cores using:
    * One or two Genesis controllers connected to the DB9 IO port or an adapter with two DB9 inputs.
    * One or two NEOGEO/Supergun controllers connected through an adapter with one or two DB15 inputs.
* Control games using one or two native controllers (including light guns) for a given system via SNAC8 (systems that don't use DB9 require an adapter).

## DB9/SNAC8 Forks with ENCC

### Update All

The `update_all.sh` script is used to download the DB9 cores. If you don't already have it, follow the instructions on the [Update_All_MiSTer repo](https://github.com/theypsilon/Update_All_MiSTer) to get it installed.

### Setup

Following these steps will enable the forks:

1. Run the `update_all` script.
2. When the countdown appears, press `UP` to enter the settings menu.
3. Enter the `Main Distribution` submenu.
4. Toggle `Cores versions` to `DB9 / SNAC8 forks with ENCC`.
5. Select `BACK` to return to the main menu.
6. Run the `SAVE` option to save your changes.
7. Run the `EXIT and RUN UPDATE ALL` option to update your mister and grab the DB9 cores.
8. Once `update_all` has finished, you should have a `UserIO Joystick` option in compatible cores.

For more information, read the [Update_All_MiSTer SNAC8 Wiki Entry](https://github.com/theypsilon/Update_All_MiSTer/wiki#snac8).

## DB9 User IO

In compatible cores you'll find the following options (some cores have them buried in a submenu):

* `UserIO Joystick`: This can be set to:
    * `DB9MD`: Use genesis controllers plugged into the DB9 port(s).
    * `DB15`: Use NEOGEO controllers plugged in to the DB15 port(s).
    * `Off`: Use other input devices for both players.
* `UserIO Players`: This can be set to:
    * `1 Player`: Configures the first DB9/DB15 port as the first player (or second player if joysticks are swapped).
    * `2 Players`: Configures the first and second DB9/DB15 ports as the first and second players.

Some cores also have a `Buttons Config` option, which let's you swap between button mapping layouts for Genesis controllers. To view the controller mappings for compatible cores, scroll to the bottom of the [MiSTer_DB9 Repository readme](https://github.com/antoniovillena/MiSTer_DB9/blob/master/readme.md).

**NOTE**: The `MinimigDB9` core has DB9 support enabled by default and lacks the options listed above.

## SNAC8

To use native controllers for a given system:

1. Connect the appropriate adapter to the DB9 port (if required).
2. Connect one or two native controllers.
3. Find the `Serial` option in the menu for the respective core and set it to `SNAC`.
4. Compatible cores will show a `SNAC Mode` option that can be set to:
    * `1 Player`: Configures the first SNAC port as the first player (or second player if the joysticks are swapped).
    * `2 Players`: Configures the first and second SNAC ports as the first and second players.
