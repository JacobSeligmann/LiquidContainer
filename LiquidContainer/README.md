# LiquidContainer

The LiquidContainer widget is a souped-up linear gauge. Instead of showing the level statically, it sports a scrolling level image. Use it to add a little pizazz using dynamic gradients, waves or whatever strikes your fancy.

The LiquidContainer consists of two main parts, the container image and liquid image. The container image must have a transparent section that serves as a viewport through which the liquid image is shown. The liquid image should be at least the size of the viewport and have matching left and right sides for smooth wrap-around when scrolling. For demonstration purposes, the LiquidContainer has a text displaying the current level and supports level adjustment by clicking (top half to increase, bottom half to decrease, in user-specified increments; this can easily be disabled or changed).

Caveat: The LiquidContainer represents my first forays into TouchGFX programming. As you can undoubtedly tell, my C++ coding skills are somewhat rusty. But hey, the code compiles and the widget seems to work, so I thought I might as well share it. Enjoy!
#TouchGFX Version
This widget was created and tested using TouchGFX version 4.4.1.
#Functional description
The initialization function takes more parameters than you can shake a stick at, but don't despair. Once your widgets are up and running, they are completely maintenance free, providing you with years of uninterrupted, carefree clicking and scrolling. So play around with the values in the examples below and see how it affects the behavior. Soon, you will be tweaking widgets like a pro.

	// show beaker
	ClickListener<LiquidContainer> beaker;
	beaker.init(BITMAP_BEAKER_ID, BITMAP_ACID_ID, 20, 250, 3, T_MILLILITERS, 39, 138, 150, 50, 0, 250, 90, 5);
	beaker.setXY(20, 20); 
  	add(beaker);

	// show test tube
	ClickListener<LiquidContainer> tube;
	tube.init(BITMAP_TESTTUBE_ID, BITMAP_WATER_ID, 25, 194, -1, T_PERCENT, 5, 159, 50, 50, 0, 100, 75, 1);
	tube.setXY(282, 55);
	add(tube);

	// show oil gauge
	ClickListener<LiquidContainer> gauge;
	gauge.init(BITMAP_GAUGE_ID, BITMAP_OIL_ID, 35, 135, 1, T_DEGREES, 0, 60, 200, 50, 90, 150, 105, 5);
	gauge.setXY(375, 60);
	add(gauge);
