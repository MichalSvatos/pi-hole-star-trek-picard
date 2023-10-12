![Pi-hole Star Trek Picard LCARS Theme](https://github.com/MichalSvatos/pi-hole-star-trek-picard/raw/main/previews/pi-hole-star-trek-picard-lcars.png)
***

# Pi-hole Star Trek Picard LCARS Theme

LCARS Theme for [Pi-hole](https://github.com/pi-hole/pi-hole) dashboard. Written completely from scratch.

***
<h1 align="center">Announcement</h1>

|                                                                                        🎉 🎉 🎉                                                                                        |
|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
| **I'm honored to announce that my Picard LCARS theme will be a part of the Pi-hole open-source project as an additional new official theme with the next update!<br/>Thank you guys!** |
|                                             The plan is to keep this repo alive and updated. You'll still be able to install it manually.                                              |


## Installation
#### ℹ️ This theme replaces the original blue LCARS theme
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

## Preview
![Pi-hole Star Trek Picard LCARS Theme Dashboard Preview](https://github.com/MichalSvatos/pi-hole-star-trek-picard/raw/main/previews/pi-hole-star-trek-picard-lcars-showcase.png)

## Gecko browsers (Firefox, Mullvad, LibreFox ... )
- Some cosmetics, such as login error and same height of the top tables on dashboard, don't work due to the lack of `:has()` support

***

## Do you prefer more colorful LCARS?
Check my other theme
[![Pi-hole LCARS Next Generation Theme](https://github.com/MichalSvatos/pi-hole-star-trek-picard/raw/main/previews/pi-hole-tng-lcars.png)](https://github.com/MichalSvatos/pi-hole-lcars-next-gen)

***

## Changelog
**1.4.2**
- FIX - checkboxes and radios for both `lcars` classes
- FIX - more general selector for footer styling `.list-inline` --> `ul[class*="list-"]`
- FIX - alert colors, border-radius and close button styling

**1.4.1**
- FIX - colored log has actually colors
- FIX - menu and login buttons tweaks (padding + overflow, ellipsis)

**1.4.0**
- **A couple of changes I made to unify the coding standards with the [Pi-hole/AdminLTE](https://github.com/pi-hole/AdminLTE/) (see [announcement](#announcement))**
  - NEW - Tabs &rarr; spaces
  - NEW - Added `.editorconfig`
- FIX - The height of the QUERY TYPES and UPSTREAM SERVERS graph box on the dashboard is now dynamic + mobile version update
- FIX - Sidebar spacing and round corners while using fluid layout
- FIX - Notification number in the header aligned properly to the side
- FIX - Network table hostname link color (for better readability)
- FIX - FOOTER on Docker version (shameless self promo removed)
- FIX - added min-height to `.content` to avoid incorrect footer position when TOOLS menu is open
- FIX - corrected position of the "timer" number in the right corner (boxed vs fluid layout)
- FIX - showed icons in the 4 status boxes on dashboard on mobile

**1.3.2**
- Add `color-scheme: dark` to avoid problems with browser's "Force dark mode" option (copy of the commit [7c2ebef](https://github.com/MichalSvatos/AdminLTE/commit/7c2ebef62b4c79844afed24e5b61d698e93618f1) )

**1.3.1**
- FIX - Scrollbar colors for CLIENTS `select2`

**1.3.0**
- NEW - Completely redesigned much cooler looking FOOTER
- FIX - Dynamic `border-radius` of the main sidebar through custom property

**1.2.1**
- FIX - scrollbar colors

**1.2.0**
- NEW - SETTINGS / PRIVACY added LCARS panel
- NEW - SETTINGS / WEB INTERFACE added LCARS panels
- FIX - SETTINGS / WEB INTERFACE input and select styled
- FIX - SETTINGS / DNS inputs styled

**1.1.0**
- NEW - DOMAINS page visual tweaks
- NEW - updated _danger area_ on SYSTEM page with new animations
- NEW - _Status_panel-47a_ updated with colors reflecting the actual state (active/disabled)
- NEW - DISABLE BLOCKING / CUSTOM TIME modal window styled
- FIX - DOMAINS page - checkbox labels on one line
- FIX - _Show X entries_ vertical align
- FIX - _Pagination_ margins
- FIX - In some _dataTables_ added rounded corners to buttons (= not visually connected to other elements)

**1.0.1**
- 🧹🗑️ Cleaning, tiny refactoring

**1.0.0**
- Version 1.0.0 released!
- NEW - updated preview

<details>
	<summary>Pre-release versions log</summary>

**0.7.2**
- Code cleaning

**0.7.1**
- FIX - Network overview table

**0.7.0**
- Network overview table

**0.6.0**
- Code cleaning

**0.5.0**
- Datepicker

**0.4.0**
- Alert modal quick styling

**0.3.3**
- FIX - SETTINGS / DHCP table

**0.3.2**
- FIX - TOP tables border removed

**0.3.1**
- Data tables responsive tweaks

**0.3.0**
- Data tables + dropdown menus
- FIX - adjusted input border color

**0.2.2**
- Page headers

**0.2.1**
- Box footers

**0.2.0**
- Finished SETTINGS / DNS page
- `code`, `pre` styling

**0.13.2**
- Audit logs button styling

**0.13.1**
- FIX - queries tables (dashboard)

**0.13.0**
- All queries tables

**0.12.6**
- Pagination

**0.12.5**
- Main drop down menu close button

**0.12.4**
- FIX - Chart "scanner" height on Long Term Data page
- FIX - Scanner loading overlay color

**0.12.3**
- Donation bar (login, other pages) + refactoring

**0.12.2**
- Login screen - donation bar

**0.12.1**
- Login screen - error message

**0.12.0**
- Login screen

**0.11.1**
- Main drop down menu

**0.11.0**
- Forms, selects, inputs, textareas
- Select2

**0.10.2**
- FIX - Checkboxes and radios styling (because icheck-bootstrap.min.css)

**0.10.1**
- FIX - More logical color (green) for checkboxes and radios
- FIX - Renamed animation for small scanners

**0.10.0**
- SETTINGS / DNS page

**0.9.3**
- Checkboxes and radios styling

**0.9.2**
- Notification "dot"

**0.9.1**
- FIX - Tab buttons in SETTINGS section width

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

</details>

## Thanks to ...
- [meWho.com](https://mewho.com) - creator of the famous SYSTEM47 screensaver and various LCARS projects
- [Jacob Bates](https://github.com/jacobbates) for this installation process

---
### License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
