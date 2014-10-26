Stretching with kinect
======================

A little stretching exercise with Kinect.

Compilation
-----------

Load the project in Visual Studio and compile it.

Use
---------

Once you are in the standing position, tilt your body backwards until Skeleton turns green. Your shoulder must be aligned between them and try to keep your hips still.

How it works
-------------

The program gets the depth of the hip and shoulder and checks that the shoulders are away from the hip a distance given by the user. 

To ensure that the user does not perform a bad movement, the function also checks that the shoulders are aligned, leaving a margin in the alignment given by the user.

If the condition it's accomplished, the brush to paint, bones and points it's changed from red to green to provide the user a feedback.

How can you use it
-------------------

As the functionality of the program is based on a boolean function wich return true if the user is in position, you may copy the funcion `isPosition37(int distance, Skeleton skeleton)` and `SkeletonPointDepth(SkeletonPoint skelpoint)` to obtain the skeleton points depth.

Use the funciont wherever you want, for example, within an `if` statement to change colors when painting the Skeleton.
