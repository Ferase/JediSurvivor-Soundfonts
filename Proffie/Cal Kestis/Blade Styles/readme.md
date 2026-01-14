These blade styles take advantage of Fett263's Multi-Phase blade to combine all the soundfonts and colors into one preset. They require the [Alt Font](https://pod.hubbe.net/sound/alt_sounds.html) setup and [Fett263's prop file](https://www.fett263.com/proffieOS7-fett263-prop-file.html) to be active on your Proffie saber with the `FETT263_SPECIAL_ABILITIES` define in your config.
If you don't know what that means, you probably don't have it enabled on your saber.

You can find a pre-configured Alt Font soundfont directory in the main Cal Kestis folder. You use it as you would any other soundfont.

Included are 4 different styles, 3 for the main blade and 1 for the crossguard quillions. The three main styles are the same, except for the different Interactive Blast configurations.

The base styles are Fett263's Cal Kestis Survivor styles, with updated colors I extracted from the game and hand-tweaked for better accuracy.

To cycle between the different colors/fonts, you just need to hold down the power button (or alt button, if you have one) on your saber and twist left or right to move forward or backward through the list, respectively. Doing so while the blade is on will instantly change the font/color, while doing it while the blade is off will change to the next color while igniting the blade.

`cal_kestis_survivor_no_interactive_blast` is the standard blade style and doesn't require any additional sound files or configuration.

`cal_kestis_survivor_single_interactive_blast` and `cal_kestis_survivor_continuing_interactive_blast` require `blast.wav` in the soundfont directory in addition to the `blst.wav` files, as well as the `EFFECT_INTERACTIVE_BLAST` define in your config. You can find more information about Interactive Blast [here.](https://www.fett263.com/proffieOS7-intro.html#blast)

These blades have alternate `party_mode` styles, which include an option to toggle swings changing the style/font of the blade, as seen in the game. This option is toggled by special ability 3 and 4 (refer to the prop file to see the bindings for special abilities).

`cal_kestis_survivor_quillion` is for the crossguard quillions, the color change function will not work without the main blade style enabled in the same preset.

All the blade styles were created in Fett263's [Style Library configurator](https://www.fett263.com/fett263-proffieOS7-style-library.html) and all copyright information is preserved in the comments of the blade style. They were designed for ProffieOS 7.15, and may not work on older versions.