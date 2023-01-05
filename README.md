# math-projectile
math projectile


The motion of a projectile can be described by the following two equations:

````
x = x0 + v0 * cos(θ) * t
y = y0 + v0 * sin(θ) * t - (1/2) * g * t^2
````

Where:

x and y are the final position of the projectile.
x0 and y0 are the initial position of the projectile.
v0 is the initial velocity of the projectile.
θ is the angle at which the projectile is launched.
t is the time elapsed since the projectile was launched.
g is the acceleration due to gravity (9.8 m/s^2).

These equations assume that the acceleration due to gravity is constant and that there is no air resistance. They are only valid for relatively short distances and low speeds.


## example 1

Suppose we want to know the position of a projectile launched from the ground with an initial velocity of 50 meters per second at an angle of 45 degrees. We can set the initial position of the projectile to (0,0) since it is launched from the ground. The acceleration due to gravity is 9.8 m/s^2.

If we let t = 1 second (the time elapsed since the projectile was launched), we can calculate the final position of the projectile using the formulas above:

````
x = 0 + 50 * cos(45) * 1 = 35.36 meters
y = 0 + 50 * sin(45) * 1 - (1/2) * 9.8 * 1^2 = 35.36 meters - 4.9 meters = 30.46 meters
````

So, after 1 second, the projectile will be at the position (35.36 meters, 30.46 meters).



## example 2

If the initial velocity of the projectile is 1073.01 meters per second and we want to know its position after a certain amount of time has elapsed, we can use the projectile motion formulas to calculate it.

Here is an example of how to do this:

Suppose we want to know the position of a projectile launched from the ground with an initial velocity of 1073.01 meters per second at an angle of 45 degrees. We can set the initial position of the projectile to (0,0) since it is launched from the ground. The acceleration due to gravity is 9.8 m/s^2.

If we let t = 1 second (the time elapsed since the projectile was launched), we can calculate the final position of the projectile using the formulas above:

````
x = 0 + 1073.01 * cos(45) * 1 = 761.61 meters
y = 0 + 1073.01 * sin(45) * 1 - (1/2) * 9.8 * 1^2 = 761.61 meters - 4.9 meters = 756.71 meters
````

So, after 1 second, the projectile will be at the position (761.61 meters, 756.71 meters).

You can use these formulas to calculate the position of the projectile at any time by substituting the appropriate value for t.


## python code

````
#!python
import math

def projectile_motion(x0, y0, v0, theta, t, g=9.8):
    x = x0 + v0 * math.cos(theta) * t
    y = y0 + v0 * math.sin(theta) * t - (1/2) * g * t**2
    return (x, y)

# Example: Calculate the position of a projectile launched from the ground with an initial velocity of 50 m/s at an angle of 45 degrees after 1 second.
x0, y0, v0, theta, t = 0, 0, 50, math.radians(45), 1
x, y = projectile_motion(x0, y0, v0, theta, t)
print(f"After {t} seconds, the projectile is at position ({x:.2f} meters, {y:.2f} meters)")
# Output: After 1 seconds, the projectile is at position (35.36 meters, 30.46 meters)

````
