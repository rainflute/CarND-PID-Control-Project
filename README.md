# Reflection

## Effects of PID controllers
1. With only P controller, the car overshoots off the middle lane and oscillate pretty badly  Here's the [link to my video result](./video/p_controller.mov)
2. D controller comes to decrease the oscillation, but if we only have D ontroller, the steer angle doesn't change much because the initial angle is ver small and the cte changes slowly too.Here's the [link to my video result](./video/d_controller.mov)
3. I controller is to fix any system bias. Integral controller results in larege steering angle when when applied alone.Here's the [link to my video result](./video/i_controller.mov)

## Hyperparameters
Twiddle doesn't work well here because I couldn't run the simulation repeatly with the code. So I decided to tune by hand based on the parameters provided in lecture.
1. Kp can be tuned alone by observing the oscillation of the car, the smaller oscillation the better result
2. Kd can be tuned after kp is tuned. It reduces the oscillation
3. Ki is tuned at last to stablelize the car, because error is cumulated, Ki should start from low value.


