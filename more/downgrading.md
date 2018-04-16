---
title: Downgrading to 1.4
layout: single
sidebar:
  nav: "side"
---

Downgrading to 1.4 allows for you to use flashcards such as the Acekard 2i which was blocked in later firmwares. This firmware is recommended as it also gets you ready to install CFW on your console when it releases, which only supports firmware version 1.4.

You must have a homebrew entrypoint before downgrading. Follow the main guide to install homebrew.

The instructions on this page will include modifying your console's internal storage (NAND). You alone will be responsible if anything bad happens to your console.

## Downloads
- twlnf 1.4 installation script
  - [USA](/assets/files/install-1.4-USA.nfs)
  - [EUR](/assets/files/install-1.4-EUR.nfs)
- [NUSDownloader](/assets/files/NUSDownloader.zip)

## Preparing
1. Make a NAND backup through twlnf and copy `nand.bin` from the root of your SD card to your computer
  - If you already made a NAND backup through twlnf, just copy the `nand.bin`
  - Do not lose this file! It is very important!
2. Open NUSDownloader on your omputer
3. Check the "Create Decrypted Contents (*.app)" box
4. Select **Database > System (DSi) > System Menu (Launcher) > [Your Region] > v512 > Start NUS Download!**
5. When done, select **Database > System (DSi) > Nintendo DS Cart Whitelist > All > v256 > Start NUS Download!**
6. When done, select **Database > System (DSi) > System Settings > [Your Region] > v512 > Start NUS Download!**
7. When done, select **Database > System (DSi) > Version Data > [Your Region] > v4 (China) > Start NUS Download!**
8. Exit NUS Downloader
9. Run `sort.py` to prepare the titles for installation
10. You now have a new folder called `title` in your NUS Downloader directory
11. Copy the `title` folder to the root of your SD card.
12. Copy the twlnf installation script for your region to the root of your SD card
13. Eject your SD card and insert it into your console

## Downgrading
1. Ensure your DSi is plugged in throughout downgrading
2. Open your homebrew entrypoint and run twlnf
3. Press **X** to mount the NAND
  - twlnf does not list this as an option
4. Navigate to the twlnf 1.4 installation script
5. Press **A** to run it
6. When the script is completed, twlnf will show `execution returned 0`
7. Press **Select** to quit twlnf
8. Press **A** to confirm
9. Your console will power off

Your console should now be on 1.4. Check in System Settings for your version, it should be 1.4 now.