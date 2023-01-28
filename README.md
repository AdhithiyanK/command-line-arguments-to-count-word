# command-line-arguments-to-count-word
## AIM:
To write a python program for getting the word count from the contents of a file using command line arguments.
## EQUIPEMENT'S REQUIRED: 
PC
Anaconda - Python 3.7
## ALGORITHM: 
### Step 1:
Import sys library
### Step 2: 
 Initialize a variable count = {}

### Step 3: 
Open the file using with open(sys.argv[1], 'r') as f:
### Step 4:  
Use for loops
### Step 5: 
Use if else to count the words

### Step 6:
End the program
## PROGRAM:
```python
import sys
count = {}
with open(sys.argv[1], 'r') as f:
    for line in f:
        for word in line.split():
            if word not in count:
                count[word] = 1
            else:
                count[word] += 1
print(count)
f.close()
```
### OUTPUT:
![Screenshot_20230128_091907](https://user-images.githubusercontent.com/121029258/215275998-7e9f7c92-826b-4be5-ac96-08080f461d37.png)



## RESULT:
Thus the program is written to find the word count from the contents of a file using command line arguments.
