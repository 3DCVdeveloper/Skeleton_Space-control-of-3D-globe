# Skeleton_Space-control-of-3D-globe
Space control of 3D globe

Development process: (Explain the development environment used: C++, tools: Windows vs2015 platform, open source libraries should be legal and indicate: openCV, openGL)
1. Functional Design - Three dimensional globe remote control based on gesture recognition (zoom in/out, spatial rotation, left/right page flipping)
2. SDK Function Development - Acquisition of Deep Data, Body Frame Data, and Joint Point Data for Astras SDK
3. Algorithm Design - Using OpenCV's imshow to display depth data and the positions of the main body joints, based on the three-dimensional coordinates of the joints and combined with flow data, design a logical algorithm for hand movements, pass different parameters to OpenGL, and use OpenGL to display the spatial transformation of the globe.
4. Writing algorithms, implementing algorithms - mainly through the coordinate transformation of three-dimensional joint points between image frames to achieve logical operations such as zooming in, zooming out, rotating, and flipping pages. In the middle, it is necessary to combine the gesture posture changes of both hands, the speed and direction changes during the gesture movement, and the relative pose changes of hand joints and other body joints to form multiple different logical judgments. After that, a certain scalar change amount is given to openGL, and openGL implements the final function based on the received scalar.
