# Memoracion-Programming-Assignment-2

# 📝 Instructions (PA 2)

## 🧮 Normalization Problem
**`import numpy as np`** uses the numpy library in order to use its functions.

- The 5x5 random array with values between 0 and 1 is created using `np.random.random((5,5))`, which is then stored into the variable **`X`**.
- `X.mean()` gets the mean value of all the elements in the array stored in **`X`**.
- `X.std()` gets the standard deviation of all the elements in the array stored in **`X`**.
- According to the formula, Subtract X by `X.mean()` then divide by `X.std()` and store it to a variable **`Z`**.

Once done, `np.save("X_normalized", Z)` is used to create a .npy file titled "X_normalized.npy" of the Z array.

---

## ➗ Divisible by 3 Problem
**`import numpy as np`** uses the numpy library in order to use its functions.

- `np.arange(1, 101)` creates an array from 1 to 100 (101 is exclusive from the array) and it is stored in a variable **`num`**
- `**` is used as an exponentiator, `num ** 2` is done to exponentiate every element in **`num`**, it is then stored to a variable **`squared`**
- `squared % 3 == 0`checks if an element in the variable **`squared`** is divisible by 3, it returns a boolean value
- `squared[condition]` selects only the elements from squared where the condition is True. Lists the value if it is true, else, it doesn't list, then stores it to the variable **`div_3`**

Once done, `np.save("div_by_3", div_3)` is used to create a .npy file titled "div_by_3.npy" of the div_3 array.
