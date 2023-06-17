# Problem statement
Shift the Center in the way that it lies on the origin $O(0, 0)$.

*Hypotheses: We have the information that* $(\bar{x}, \bar{y})$ *is the center coordinate.*

# Solution

To recenter a dataset with a known center at coordinates $(\bar{x}, \bar{y})$ and shift it to have the center at the origin (0, 0), you can subtract the center coordinates from each data point.

Here's how you can recenter the dataset:

1. Let $n$ be the total number of data points in the dataset, $(x_i, y_i)$ represent the coordinates of the $i$-th data point and center coordinates is the point $(\bar{x}, \bar{y})$.

2. Subtract the center coordinates $(\bar{x}, \bar{y})$ from each data point to recenter the dataset:

   $$(x_i', y_i') = (x_i - \bar{x}, y_i - \bar{y})$$

This will shift the dataset so that the new center lies on the origin $O(0, 0)$.

