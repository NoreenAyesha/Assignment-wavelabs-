# Assignment-wavelabs

To solve this problem, you can start by iterating over all the possible integral coordinates on the X-Y plane within a certain range. For each coordinate, calculate the network quality by iterating over all the towers and checking if the distance between the tower and the coordinate is less than or equal to the given radius. If it is, then add the signal quality of that tower to the network quality.

Once you have calculated the network quality for all the possible coordinates, you can find the maximum network quality and return the corresponding coordinate. If there are multiple coordinates with the same network quality, you can return the lexicographically minimum non-negative coordinate.
The network_tower function takes in the towers and radius as inputs and returns the coordinate with the maximum network quality. The max_quality and max_coord variables keep track of the maximum network quality and the corresponding coordinate so far.
