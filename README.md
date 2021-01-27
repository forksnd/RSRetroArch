# RSRetroArch
 (Curated) Repository of RetroArch and retro-related shaders / shaders from programs, ported for ReShade.
 If you like what you see, consider dropping a coin at my PayPal at that email: matsilagi2@hotmail.com. Any amount is appreciated.
 
 Also to be soon refactored is my (mostly grey-area) Unity shaders repository, so stay tuned!

#### CONTENTS
 The Shaders included here comes mostly from [libretro/common-shaders](https://github.com/libretro/common-shaders) , but there are some from other sources aswell, below are a list of shaders, where they came from, and what they do:
 - 3DFX by LeiLei: attempts to mimic the VGA / RAMDAC cables, color dithering and screen quality of 3DFX cards, more specifically Vooodoo 2/3. Long gone from the RetroArch Shader repository.
 - ArtifactColors by FlyGuy: Uses a signal modulation created trough NTSC artifacting, to generate colors, pretty much like Apple II's low-res mode.
 - CMYK Halftone Dot by hunterk: Originally made as a WebGL Demo by Stefan Gustavson, simulates the halftone dots used in CMYK prints, useful for magazine-like shots.
 - CoolRetroTerminal by Swordfish90: Originally from a Linux app [Swordfish90/cool-retro-term] (https://github.com/Swordfish90/cool-retro-term) , i ported its Pixel Shader from QT a long time ago, its not by any means up-to-date, but still looks ultra-similar to how CoolRetroTerm works so, i guess its still useable. A big buggy and without bloom, but most of its features work fine.
 - CRT-Aperture by ???: Couldn't find the Author name, but seems like a modified CRT-Easymode made to mimic more a Trinitron display.
 - CRT-Caligari by Caligari: A port made by Hyllian of an experiment made by Caligari. Based on xythen's Matlab algorithm on a scale-factor independent CRT shader.
 - CRT-cgwg by cgwg and Themaister: One of the oldest CRT shaders, made to mimic a slotmask CRT. It was the base work for lots of future implementations, and considered to be the pioneer on that extent / niche.
 - CRT-Easymode by Easymode: A fast / lightweight flat-display CRT shader intended for 1080p displays. Not that fancy, but it looks good and with a average perf. hit when Graphics Power is of concern.
 - FakeLottes by hunterk: A scanlines + crt curvature shader using Lottes masks. Used as an alternative to CRT-Lottes for low power GPUs and Raspberry systems.
 - CRT-Geom by cgwg, Themaister and DOLLS: A modified / further worked CRT shader based on cgwg. Has more options for masks, distortions and rotations of the CRT display. Meant to mimic Arcade-machine cabinets and displays.
 - CRT-Hyllian by hyllian: A sharp / Trinitron-like CRT Shader. Made to give a sharp and crisp output with slight bloom, similar to Sony's BVM line of displays.
 - CRT-Lottes by Timothy Lottes: Created by the same person who made FXAA for nvidia, this is a high-quality and good looking CRT shader for 1080p and larger displays. Requires a somewhat powerful PC to run it, has multiple mask and distortion options, Bloom and Halation effects. Used in the book "The Bitmap Brothers: Universe" for the images on it.
 - CRT-Lottes 2.0 by Timothy Lottes: A revision / update of his previous work. Has a bit of less features, works a bit differently, but its still an amazing CRT shader candidate for 1080p displays.
 - CRT-NES-MINI by ???: Based on the CRT shader found on Nintendo's Retro NES console. Its incredibly lightweight, but has no fancy bells and whistles, just simple scanlines.
 - CRT-Pi by davej: A shader designed to take it easy on Raspberry Pi systems. Incredibly lightweight aswell with main characteristics of CRT displays. Should be useful for those running under integrated displays.
 - CRT-Potato by Brad Parker: Available in 2 versions (Cool and Warm), this shader takes a CRT mask texture and tiles it on the screen, making it a pretty looking CRT Phosphor Mask shader, without a very big performance hit, so light even a "potato" computer can run it.
 - CRT-Sim by Kyle Pittman: Taken from "Super Win the Game", this shader mimics a old CRT TV with the crosstalking / Dot Crawling artifacts of NTSC signal. Also has phosphor decadence effects of a CRT display.
 - CRT-Yee64 and CRT-Yeetron by Christian Whitehead: Based on a reverse-engineered / assembly version of the shaders found in Sonic Mania. Not 100% scale-accurate, but looks fine on most use-cases. Yee64 is the SMOOTH option, while YEETRON is the Sharp option.
 - EGAFilter by ???: Taken from DOSBox, meant to mimic an EGA display, with very, VERY limited color depth.
 - GTUv50 by aliaspider: Less meant to mimic the physical CRT appearance and more the signals interpreted by them, this works as a NTSC-shader with scanlines mostly. Due to its flexibility with blurring, can be easily used to fix / re-blend dithering effects in old games. Requires a somewhat-powerful PC in certain values.
 - LeiFX_OA (3DFX) by LeiLei: Same as 3DFX, but ported from OpenArena, supposedly, that one is more updated than the RetroArch versions.
 - MCAmber,Green and Orange by ???: Taken from DOSBox, made to mimic monochrome phosphor displays. It basically just tints the screen, nothing too special about them.
 - MMJCelShader by MMJuno: A port of an old shader from Pete's OGL2 plugin for ePSXe. Adds cel-shading and posterizing to the image, giving it a cartoon-ish look.
 - nGlide 3DFX by Zeus Software: A port of the experimental 3DFX dithering and RAMDAC filtering used in nGlide. It is accurate to the old GPUs and not meant to mimic them, so, lower resolutions will look better with it.
 - NTSC by Themaister and cgwg: A shader that mimics NTSC Crosstalk and signal. Comes with a few options and a variation with no scanlines for those who just want to use the signal part with another CRT shader bundled.
 - PAL by svo: A shader which mimics the signal of PAL displays with its artifacts and imperfections.
 - R57_PAL by r57shell: A PAL shader meant to also mimic the artifacts and dot crawling of the PAL signal. Comes with 2 versions, the new one is actually using the r57 pal preset for any system, and the old one is like defining USE_SAMPLED and USE_RAW on the preset.
 - RetroCRT by KillaMaaki: A port of the CRT shader from PPSSPP. Has color distortions, scanlines and barrel / display distortion.
 - Scanlines-Abs by RiskyJumps: A sine-wave Scanline shader. Applies scanlines using a Sine-Wave, looks great with integer scaled games.
 - Scanlines-Fract by hunterk: Similar to the Scanlines-Abs, but using a frac operation. May look thicker and darker on some cases, but works better with non-integer scaled games.
 - Technicolor by hunterk: A Technicolor shader meant to mimic old cartoons and suchs. Inspired partly by Cuphead.
 - zfast_crt by SoltanGris42: An ultra-lightweight CRT shader. Made to work fast on integrated gpus, while looking good. Designed for 1080p displays.
 
 There are also a few shaders from MAME included, those are:
 - ColorMAME: Meant to work as a color-tweaking knob of a CRT display. Part of the MAME CRT shader, but split-out for convenience.
 - Deconverge: Meant to simulate color convergence on CRT Displays. Distorts the channels of the image.
 - Defocus: Meant to simulate the blurring of a CRT display. Blurs the image Horizontally and Vertically, similar to a Gaussian Blur shader.
 - NTSC: A direct port of MAME's NTSC signal emulation shader. Works similar to the one by Themaister, but with non-animated crosstalk and less saturated colors.
 - Phosphor: Simulates the phosphor decadence of a CRT display, leaving "ghosts" of the previous frames.
 
 And also, some more experiments ported from around the web and Shadertoy
 - BasicCRT by the8bitpimp: A really basic blue / frosted-glass like CRT shader with flickering. (https://the8bitpimp.wordpress.com/2014/07/17/retro-crt-shader/)
 - Cathode by nimitz: Creates a shadowmask / grid similar to a CRT display. (https://www.shadertoy.com/view/4lXcDH)
 - LCD Post Effect by MenacingMecha: Makes the screen look like a Backlit LCD display, not really useful but might look eye-candy for some (https://www.shadertoy.com/view/ldBfDd)
 - MattiasCRT by Mattias: Ported from Shadertoy (https://www.shadertoy.com/view/lsB3DV) , based on the work of inigo quilez.
 - MetaCRT by P_Malin: Phosphor Mask / 2D part of the MetaCRT Shadertoy by P_Malin (https://www.shadertoy.com/view/4dlyWX)
 - Needs More JPEG by rory618: Applies DCT compression used by the JPEG file format. (https://www.shadertoy.com/view/llfyz4)
 - NTSC Decoder by XOT: Modulates the signal like NTSC does. (https://www.shadertoy.com/view/Mdffz7)
 - TV CRT Pixels by iq: Mimics the Shadow-Mask / Slot-Mask of a CRT TV. (https://www.shadertoy.com/view/XsfGDl)
 - vt220 by sprash3: Meant to mimic a vt220 terminal, also includes the Night version + a version with the Frame only so you can fit your own screen data inside it. (https://www.shadertoy.com/view/MtBXW3)

#### PARTNER REPOSITORIES

Those repositories might also have something you like, make sure to check them out!
 [akgunter/crt-royale-reshade] (https://github.com/akgunter/crt-royale-reshade) - A port of the most accurate and feature filled CRT shader of RetroArch for ReShade. Original work by TroggleMonkey, ReShade port by akgunter.
 [luluco250/FXShaders] (https://github.com/luluco250/FXShaders) - luluco's shader repository. Probably listed at the big ReShade ones, but worth mentioning here.
	 
#### CREDITS

 Besides the ones from their original authors, a few goes for me. Mostly for porting, fixing and maintaining those over the years. It was due to a reformulation / re-organization so it could get curated and pasted onto the reshade repositories list.
 Since i was considered the "Retro-shaders" guy for ReShade, i decided to fully embrace it and include shaders from my misc repos and Shadertoy Repos related to that sort of thing. This was the result.
	
 Also credits to Pascal Gilcher and luluco250 for helping me with stupid questions i had back at the time, and basically tutoring / mentoring me. Also thanks to akgunter for fixing CRT-Potato for me last night.
