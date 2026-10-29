# Background presets and hashtag footer

Version 0.5 includes four selectable preview cards in Appearance:

| Preset | Display colors |
| --- | --- |
| Guide blue | `#21409A`, white accent |
| Blue gradient | `#21409A` to `#101E4A`, white accent |
| Dark blue | `#101E4A`, white accent |
| White & blue | White, `#21409A` accent |

The selected preset is saved in the tournament file. Selecting one clears a custom background image so the chosen preset is visible. It preserves logos, dimming and the staff-image preference. Editing the custom color switches back to a plain color. Custom event images remain available through Choose image.

## IJF reference and scope

Source checked on 26 October 2026: the [IJF Event Organization Guide](https://78884ca60822a34fb0e6-082b8fd5551e97bc65e327988b444396.ssl.cf3.rackcdn.com/up/2023/03/2017_IJF_EOG_version_6_03_2017-1678371927.pdf), linked from the [official IJF documents page](https://www.ijf.org/documents). The linked filename identifies the 2017 guide; its relevant pages carry an Edition 1.1 February 2015 footer.

Section 1.5, page 10, specifies dark blue for banners with C100 M90 Y20 K0, and says World Championship colors are agreed with the IJF. The blue vector text in that PDF uses RGB approximately `#21409A`, which supplies the screen reference here. This is a display approximation, not a color-managed proof of the print formula. The gradient, dark and white variants are application layouts based on that palette. They do not include IJF logos or sponsor allocations and do not constitute event approval. Import the event's approved artwork when supplied.

## Hashtag footer

The optional Event hashtag is tournament data, independent of the staff appearance checkbox. It appears on both audience and staff output. Missing leading `#` characters are added to space-separated tokens. The footer uses a reserved bottom row; rising flags are clipped above it. The bottom-center logo moves upward to keep the text clear. Leave the field empty for the earlier layout.

Hashtags and presets are captured in the loaded ceremony snapshot. Preparing another category or appearance does not change a live ceremony. Blackout hides the footer along with the flags and logos.
