# LiquidContainer

The LiquidContainer widget is a souped-up linear gauge. Instead of showing the level statically, it sports a scrolling level image. Use it to add a little pizazz using dynamic gradients, waves or whatever strikes your fancy.

The LiquidContainer consists of two main parts, the container image and liquid image. The container image must have a transparent section that serves as a viewport through which the liquid image is shown. The liquid image should be at least the size of the viewport and have matching left and right sides for smooth wrap-around when scrolling. For demonstration purposes, the LiquidContainer has a text displaying the current level and supports level adjustment by clicking (top half to increase, bottom half to decrease, in user-specified increments; this can easily be disabled or changed).

Caveat: The LiquidContainer represents my first forays into TouchGFX programming. As you can undoubtedly tell, my C++ coding skills are somewhat rusty. But hey, the code compiles and the widget seems to work, so I thought I might as well share it. Enjoy!
