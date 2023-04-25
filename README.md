# Assignment-wavelabs

To solve this problem, you can start by iterating over all the possible integral coordinates on the X-Y plane within a certain range. For each coordinate, calculate the network quality by iterating over all the towers and checking if the distance between the tower and the coordinate is less than or equal to the given radius. If it is, then add the signal quality of that tower to the network quality.

Once you have calculated the network quality for all the possible coordinates, you can find the maximum network quality and return the corresponding coordinate. If there are multiple coordinates with the same network quality, you can return the lexicographically minimum non-negative coordinate.
The network_tower function takes in the towers and radius as inputs and returns the coordinate with the maximum network quality. The max_quality and max_coord variables keep track of the maximum network quality and the corresponding coordinate so far.

Input:
3
-2 2 4
1 1 3
3 3 1
4
Output:
0 0

Explanation:
The reachable towers from (0, 0) are the towers at (-2, 2) and (1, 1), as they are both within a distance of 4. The signal quality for these towers at (0, 0) is calculated as follows:

For tower at (-2, 2), d = sqrt((-2-0)^2 + (2-0)^2) = sqrt(8) and q = floor(4 / (1 + sqrt(8))) = 1
For tower at (1, 1), d = sqrt((1-0)^2 + (1-0)^2) = sqrt(2) and q = floor(3 / (1 + sqrt(2))) = 1
The network quality at (0, 0) is the sum of these signal qualities, which is 1 + 1 = 2. Since this is the maximum network quality possible, the output is [0, 0].

NOTE* The shared code is best ran on https://www.programiz.com, for accurate output :)


