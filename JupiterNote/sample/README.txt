This small sample data set contains signature data collected from
five users.  For each user, there are 20 genuine signatures and
20 skilled forgeries.

Each genuine/forgery signature is stored in a separate text file.
The file names are in the format "USERx_y.txt", where x (1..5)
indicates the user and y (1..40) indicates one signature instance
of the corresponding user, with the first 20 (1..20) representing
genuine signatures and the rest (21..40) representing skilled
forgeries provided by the other users.

In each text file, the signature is simply represented as a
sequence of points.  The first line stores a single integer which
is the total number of points in the signature.  Each of the
subsequent lines corresponds to one point characterized by seven
features listed in the following order:

  X-coordinate  - scaled cursor position along the x-axis
  Y-coordinate  - scaled cursor position along the y-axis
  Time stamp    - system time at which the event was posted
  Button status - current button status (0 for pen-up and
                  1 for pen-down)
  Azimuth       - clockwise rotation of cursor about the z-axis
  Altitude      - angle upward toward the positive z-axis
  Pressure      - adjusted state of the normal pressure
