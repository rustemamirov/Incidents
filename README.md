# Incidents
Processing an array of incidents according to a complex algorithm

There is a set of N incidents. Each has: id with consecutive values from 0 to N-1, two categorical signs with integer values from 0 to M-1, a sign of time with some (non-integer) value from 0 to 1.

It is necessary to write to the function that receives the input dT and the file with the incidents, and for each of the N incidents it calculates the number of incidents that satisfy the following conditions:

- precede the incident in time, with the time difference not exceeding dT;
- have the values of feature1 and feature2, coinciding with the corresponding values of the incident.

The function should read the csv-file with incidents, calculate the results for all incidents and write them into a csv-file of the specified type. The main nuance: the function should work quite quickly, namely, no longer than a minute with M = 100, N = 1,000,000, dT = 0.3.
