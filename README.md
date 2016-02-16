# 3d-vision

## Self-calibrated Stereoscopic 3D Vision System Using Off-the-shelf Digital Cameras. 

Written by Jacobo Rouces <jacobo@rouces.org>.

This is my Bachelor project, which I did several years ago (2009), and I have decided to make open-source in case someone can make good use of it. Adapted from the abstract:

It is a software system that makes use of stereoscopic vision through cheap off-the-shelf cameras, to offer a tridimensional Human Interface Device. In other words, the computer knows in real time the three-dimensional coordinates of a device held by the user, by using two or more webcams. So that the tracking may be done in real time, the devices are led lights (the real-time system uses low exposure to locate them easily). The more cameras, the more accurate is the min-square approximation of the position, and the more resilient to occlusion by the user's body the system becomes. The system is able to work with different kinds of cameras in any relative positions and orientations (as long as they are different enough to be well formed). The system automatically infers the parameters for this when the user holds a simple 4-point pattern in front of the screen (a DIN-A4 flat sheet on a black background is the most convenient choice). It uses Newton-Raphson to approximate the parameters.

The long mathematical discussions are in the report in PDF, but unfortunately, this is only in Spanish.

The system is mostly implemented in Matlab, with some critical parts in C. I never tested it in Octave, but it might be adapted. The only fancy library I remember using was the one for video acquisition.
