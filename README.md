# python-strings
working with strings

1. Basic iteration over a string. 
```
def sample(sentence):
    
    for i in sentence:
        print(i, end='') // the ducks are in a pond
   
   
sentence = "the ducks are in a pond"
sample(sentence)
```

2. Iterate over the string using split, getting the results above
```
def sample(sentence):
    
    words = sentence.split(", ")
    
    for word in words:
        print(word) // the ducks are in a pond
   
   
sentence = "the ducks are in a pond"
sample(sentence)
```

3. Iterate over the string getting the length of each word
```
def sample(sentence):
    
    words = sentence.split()
    word_length = []
    
    for word in words:
        word_length.append(len(word))
    print(word_length) // [3, 5, 3, 2, 1, 4]
   
sentence = "the ducks are in a pond"
sample(sentence)
```

4. Using a list comprehension, iterate over the string and get the length of each word
```
def sample(sentence):
    
    words = sentence.split()
   
    word_length = [len(word) for word in words]
    
    print(word_length)
   
sentence = "the ducks are in a pond"
sample(sentence)
```

5. Using a list comprehension, interate over the string printing the words >= length of 3
```
def sample(sentence):
    
    words = sentence.split()
   
    word_length = [word for word in words if len(word) >= 3]
    
    print(word_length)
   
sentence = "the ducks are in a pond"
sample(sentence)
```

6. Iterate over a sring using range(len()) and return the letter along with its index
```
def sample(sentence):
    
    for i in range(len(sentence)):
        print(f"{i}:{sentence[i]}", end=', ')
   
sentence = "the ducks are in a pond"
sample(sentence)
```

7. Iterate over a string, split it, and return each word along with its index using range(len())
```
def sample(sentence):
    
    words = sentence.split()
    
    for i in range(len(words)):
        print(f"{i}:{words[i]}", end=', ')
   
sentence = "the ducks are in a pond"
sample(sentence)
```
