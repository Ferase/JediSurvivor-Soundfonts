# Proffie Blade Styles
Here you can find blade styles for each soundfont. There are 4 styles in each folder, 3 of which being main blade styles, and one being a quillion blade style.

## Main Blade Styles
For each soundfont there are 3 main blade styles - `no_interactive_blast`, `single_interactive_blast`, and `continuing_interactive_blast`:
### no_interactive_blast
`no_interactive_blast` is the default blade style, and requires no further setup than copying and pasting the style into your proffie config. They have statically timed blaster deflection effects, with a 150ms delay between the button press and the blade effect, which matches up with the default `blst.wav` files.
### single_interactive_blast/continuing_interactive_blast
`single_interactive_blast` and `continuing_interactive_blast` are blade styles set up to use Fett's Interactive Blast feature. The only difference between the two styles is `single_interactive_blast` requires you to press the button every time you want a blaster fired, while `continuing_interactive_blast` will continue firing until you miss a deflection.

 This requires `blast.wav` (the blaster firing sound) in the soundfont directory in addition to `blst.wav` (the saber deflection sound), as well as `EFFECT_INTERACTIVE_BLAST` defined in your config with and [Fett263's prop file](https://www.fett263.com/proffieOS7-fett263-prop-file.html). These sounds are included in the `_PROFFIE EXTRAS` folder. You can find more information about Interactive Blast [here.](https://www.fett263.com/proffieOS7-intro.html#blast)

## Qullion Blade Styles
If you have a saber with independently wired quillion blades, there are additional `quillion` blade styles in each blade style folder. These just get copied into the proffie config like you would any secondary blade style.

Cal Kestis's `quillion` style is somewhat special, in as much as it calls the quillion ignition sound when it ignites. This works through a `TrDoEffect` calling `EFFECT_TRANSITION_SOUND`, which uses `tr/01/00*.wav` for the ignition sound and `tr/02/00*.wav` as the retraction sound. What this means is that you don't have to use a baked ignition sound, and allows you to adjust the quillion ignition delay directly from the ProffieOS workbench or your `presets.ini` file. The default ignition delay is one second. A special work-in-progress/proof-of-concept style that allows you to turn the quillions off and on while the saber is on also included, `quillion_toggle_beta`, which ignites/retracts the quillions when you point the saber down, hold power, and twist left (hold aux and twist left in any orientation on dual button sabers). It generally works just fine, aside from some audio bugs.

# 'Alt Font' Styles
The Cal Kestis and Dagan Gera blade styles take advantage of Fett263's Multi-Phase blade to combine all the soundfonts and colors into one preset. They require the [Alt Font](https://pod.hubbe.net/sound/alt_sounds.html) setup and [Fett263's prop file](https://www.fett263.com/proffieOS7-fett263-prop-file.html) to be active on your Proffie saber with the `FETT263_SPECIAL_ABILITIES` define in your config (although I've heard that BC's prop might have ways to activate user effects too, but I haven't personally tried it out).
If you don't know what that means, you probably don't have it enabled on your saber.

You can find pre-configured Alt Font soundfonts in the same folder as the individual soundfonts. You copy them onto the SD card it as you would any other soundfont. Alt Fonts are standalone, and don't require the individual soundfonts to work.

To cycle between the different colors/fonts on single button sabers, you just need to turn the saber on, hold down the power button on your saber, and twist right or left to move forward or backward through the list. If you don't like the mechanical noises every time the saber changes color, you can delete the `altchng` folder from the soundfont directory. When using the Cal Kestis font, twisting right while pointing the saber down will instead activate and deactivate Party Mode, which switches the color on swing, like in the game (you'll hear some playful beeps when it's toggled). For dual buttons sabers, it doesn't matter what orientation the saber is in. Holding power and twisting will change the colors, holding aux and twisting will activate party mode.

# Credits

All blade styles were created in Fett263's [Style Library configurator](https://www.fett263.com/fett263-proffieOS7-style-library.html) and then manually modified by [crazy.hair](https://github.com/crazy-hair). All copyright information is preserved in the comments of the blade style. They were designed for ProffieOS 7.15, and may not work on older versions.