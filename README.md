![Pi-hole Star Trek Picard LCARS Theme](https://github.com/MichalSvatos/pi-hole-star-trek-picard/raw/main/previews/pi-hole-star-trek-picard-lcars.png)
***

# Pi-hole Star Trek Picard LCARS Theme

LCARS Theme for [Pi-hole](https://github.com/pi-hole/pi-hole) dashboard. Written completely from scratch.

## ℹ️ Officially part of the Pi-hole project
Since [web v5.21](https://github.com/pi-hole/web/releases/tag/v5.21) you can choose new _Star Trek Picard LCARS theme (dark)_ in _SETTINGS/WEB INTERFACE_.

***

## Manual installation
Type the following commands into SSH, line by line to install the newest version.

```
cd /var/www/html/admin/style/themes/
sudo git clone https://github.com/MichalSvatos/pi-hole-star-trek-picard.git
sudo rm -f lcars-picard.css
sudo cp pi-hole-star-trek-picard/lcars-picard.css .
sudo rm -rf pi-hole-star-trek-picard
```

⚠️ Check the trailing " ." on the 3rd line (it's not a typo - it means copy to current directory).

ℹ️ Without editing `/var/www/html/admin/settings-xxxxx.lp` pages, the SYSTEM screens will not work properly.

ℹ️ For WEB INTERFACE version older than 5.21, use `lcars.css` in the code above. That will replace the original blue LCARS theme.

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
**2.1.0**
- NEW - SAVE &amp; APPLY button
- NEW - information on `:hover` on STATUS and MEMORY panels in STATUS_PANEL_47A
- NEW - DOMAIN MANAGEMENT colored buttons and new tabs
- NEW - DONATION BAR
- NEW - ADVANCED FILTERING collapsible box
- NEW - ALL SETTING basic styling
- NEW - SETTINGS
  - DNS
  - DHCP
  - WEB/API
  - PRIVACY
  - TELEPORT
  - LOCAL DNS REPORTS
- FIX - page header + BASIC/EXPERT MODE toggle button
- FIX - box header - zoom info/reset button
- FIX - added text to "SELECT/DESELECT ALL" button (thanks to [jammmekod's issue](https://github.com/MichalSvatos/pi-hole-star-trek-picard/issues/1))
- FIX - Select2 width in CLIENT GROUP MANAGEMENT
- FIX - Second level submenu (TAIL LOG FILES)
- FIX - DOMAIN MANAGEMENT button wrap on mobile
- FIX - FOOTER - _component status_ label while sidebar is collapsed
- some unused code removed

**2.0.0 (Pi-hole v6)**
- FIX - all the bells and whistles around the boxes visible
- FIX - DROPDOWN MENU - icon sizes
- NEW - DROPDOWN MENU - new information (client, render time) styled
- NEW - MAIN MENU - labels shape and colors
- NEW - BOX HEADER - zoom info icon
- NEW - FOOTER - variant of the "INSTALLATION INSTRUCTIONS" panel when there're no updates

<details>
  <summary>v1.0.0+</summary>

**1.4.3**
- FIX - checkboxes & radios class refactoring
- FIX - removed "LCARS theme by @MichalSvatos" from main menu
- FIX - button alignment in TOOLS/AUDIT LOG table

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
</details>

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

## Like my work?️
Just **spread the word**. But if you feel like it, any donations are highly appreciated ❤️!

#### Monero
![Monero QR code](https://github.com/MichalSvatos/pi-hole-star-trek-picard/raw/main/imgs/qr-monero.png)
`82cdV2a1RU34pnv7x4tQtV4pTv1wgM5DjFEM1SQz8keF2z6ZidSbpNq51p8S3NMdYwh5PecSRBuSkAthbEmJUisoHVj6W8o`

---
### License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
