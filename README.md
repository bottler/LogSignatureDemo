#Demonstration of Log Signature calculations

This is example code for calculating the signature of a path using the method described at http://www2.warwick.ac.uk/fac/cross_fac/complexity/people/students/dtc/students2013/reizenstein/logsignatures.pdf .

logsignature.py is the same as the original distribution on [http://www2.warwick.ac.uk/fac/cross_fac/complexity/people/students/dtc/students2013/reizenstein](Jeremy's website) except you can use command-line arguments to specify the dimension (D) and level (M).

To calculate the logsignature of a random path in 3D up to level 6:

```
python logsignature.py 3 6
g++ --std=c++11 -DDIM=3 -DLEVEL=6 bch.cpp calculate.cpp
./a.out 
```

Running the python script and compiling the code will in general be slow, but the final program should be fast.