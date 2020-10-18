PES1201801708.c is the library and you can utilize it as shown in sampletest.c

Introduction:
An intal is a nonnegative integer of arbitrary length, but it is sufficient for your implementation to support up to 1000 decimal digits. 
The integer is stored as a null-terminated string of ASCII characters. An intal is represented as a string of decimal digits
that are stored in the big-endian style. That is, the most significant digit is at the head of the string.
Intal can be used to store large(in thousand digits) which is enormous even when compared with long long int of C.
Intal can be used in creating big number online calculators.Intal has various functionalities like add,multiply etc

Implementation:

1)char* intal_add(const char* intal1, const char* intal2):-The two arrays are reversed then iterated and stored by keeping carry for next iteration.Lastly the string is reversed and returned.


2)int intal_compare(const char* intal1, const char* intal2):-comparing the length of strings, if even they are same ,  they check individual digits.


3)char* intal_diff(const char* intal1, const char* intal2):-The reversed arrays are iterated and subtracted carry(if used) is later subtracted in next iteration.

4)char* intal_multiply(const char* intal1, const char* intal2):-I took each digit of multiplier, the I multiply with whole multiplicand using for loop and return required character array.


5)char* intal_mod(const char* intal1, const char* intal2):-I brought the value of intal2  close to intal1 and  then recursively substract the same and then returned that array.


6)char* intal_pow(const char* intal1, unsigned int n):-I created an array with the value =1 and   multiply every time with the intal1 until n is finished in while loop and return that array


7)char* intal_gcd(const char* intal1, const char* intal2):-Here I followed standard euclidean algorithm to find gcd.



8)char* intal_fibonacci(unsigned int n):-0 and 1 are the first two fibonacci numbers,two arrays are created, then till n is in while loop adding intial 2 values then returned our array


9)char* intal_factorial(unsigned int n):-I used recursion  until n becomes 1 .Logic is n*(n-1)*(n-2)....1.


10)char* intal_bincoeff(unsigned int n, unsigned int k):-I used dyamic approach where I created an array of size of product of 2 so that I can store the corresponding values and then returnn the required value.


11)int intal_max(char **arr, int n):-Made pointer pointing to the initil array and a index variabe  and iterating from index 1 to last and if a array bigger is found pointer and index variable is updated..later returning index


12)int intal_min(char **arr, int n):-I made  pointer pointing to the initil array and a index variabe  and iterating from index 1 to last and if a array bigger is found pointer and index variable is updated..later returning  index


13)int intal_search(char **arr, int n, char* key):-Key is compared with the  every large array,, if key is found that index is returned else -1 is returned.


14)int intal_binsearch(char **arr, int n, char* key):-The Array is  sorted and key is found in 2 halfs then index or -1 is returned.

15)void intal_sort(char **arr, int n):-Used merge sort to sort half and half arrays then merged both arrays together recursively..and old array  is copied to  new created sorted array


16)char* coin_row_problem(char **arr, int n):-Used Dynamic programming where every index is updated to max of(sum of present index value + sum of (present index-2) value,value of present index -1) then I returned last index value


