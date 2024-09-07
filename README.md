# Nariz_PA-2
This repository features Python scripts that tackle programming challenges named 'Normalization' and 'Divisible by 3.'

# 1. Normalization Problem
This code creates and displays a 5x5 array of random values and its normalized version.

```python
import numpy as np

#Create a random array that is 5 x 5
X = np.random.rand(5, 5)

#Set the values
mean = np.mean(X)
std = np.std(X)
Z = (X - mean) / std

#saving
Normalized_X = np.save("X_normalized.npy", Z)

#printing the output
print("Your current value: ")
print(X)
print("Your normalized value: ")
print(Z)
```
