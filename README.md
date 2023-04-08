![Pi-hole Star Trek Picard LCARS Theme](https://github.com/MichalSvatos/pi-hole-star-trek-picard/raw/main/previews/pi-hole-star-trek-picard-lcars.png)
***

# Pi-hole Star Trek Picard LCARS Theme

LCARS Theme for [Pi-hole](https://github.com/pi-hole/pi-hole) dashboard. Written completely from scratch.

## Installation
### ℹ️ This theme replaces the original blue LCARS theme
Type the following commands into SSH, line by line.

```
cd /var/www/html/admin/style/themes/
sudo git clone https://github.com/MichalSvatos/pi-hole-star-trek-picard.git
sudo rm -f lcars.css
sudo cp pi-hole-star-trek-picard/lcars.css .
sudo rm -rf pi-hole-star-trek-picard
```

⚠️ Check the trailing " ." on the 3rd line (it's not a typo - it means copy to current directory).

## Uninstall/Revert
Type the following commands into SSH, line by line.

```
cd /var/www/html/admin/style/themes/
sudo git reset --hard
```

## Docker installation
Run the same commands directly in the container as shown [here](https://github.com/MichalSvatos/pi-hole-lcars-next-gen/issues/1#issuecomment-1372378045).

_Note: I didn't test it myself._

## Changelog
**0.9.0**
- SETTINGS / SYSTEM page
- FIX - pulseBg animation new variable

**0.8.5**
- Tab buttons in SETTINGS section

**0.8.4**
- FIX - font weight and subpage version of STATS boxes

**0.8.3**
- FIX - removed custom FontAwesome icon. Don't ask 🤦

**0.8.2**
- FIX - colors for the JS generated content 

**0.8.1**
- FIX - same height of the "TOP" tables

**0.8.0**
- Donation bar
- Footer + update available variant

**0.7.0**
- "TOP" tables on the dashboard 

**0.6.3**
- Charts "scanner" animation

**0.6.2**
- Preview images in README

**0.6.1**
- Pie charts visual tweak (mirroring)

**0.6.0**
- Pie charts styling

**0.5.0**
- First commit containing - header, sidebar + menu, total queries, clients and user panel, basic animations

## Thanks to ...
- [meWho.com](https://mewho.com) - creator of the famous SYSTEM47 screensaver and various LCARS projects
- [Jacob Bates](https://github.com/jacobbates) for this installation process

## Do you prefer more colorful LCARS?
Check my other theme
[![Pi-hole LCARS Next Generation Theme](https://github.com/MichalSvatos/pi-hole-star-trek-picard/raw/main/previews/pi-hole-tng-lcars.png)](https://github.com/MichalSvatos/pi-hole-lcars-next-gen)

---
### License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
