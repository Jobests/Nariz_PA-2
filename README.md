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
# Output

![image](https://github.com/user-attachments/assets/9fa8b795-a26e-4813-827e-457bf312070f)

# 2. Divisible by 3 Problem
This code produces a 10x10 array where each element is the square of integers from 1 to 100. It also prints out the divisible numbers in the array by 3.

```python
import numpy as np

A = np.arange(1, 101) #Create the range of the array from 1 - 100
B = A.reshape(10, 10) #Reshape the array to 10 x 10
C = np.square(B) #Square all of the elements inside of the array
print(C) #print

#Using boolean indexing to find the values that are divisible by 3 and stores it
divisible_by_3 = C[C % 3 == 0] 

#saving
np.save("div_by_3.npy", divisible_by_3)

#Print the values that are divisble by 3
print("The values that are divisible by 3 are: ")
print(divisible_by_3)
```
# Output
![image](https://github.com/user-attachments/assets/38502858-4c00-498f-aa80-56df9aca4178)
