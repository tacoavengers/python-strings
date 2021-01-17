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

5. Using a list comprehension, iterate over the string printing the words >= length of 3
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
        print(f"{i}:{sentence[i]}", end=', ') // 0:t, 1:h, 2:e, 3: , 4:d, 5:u, 6:c, 7:k, 8:s, 9: , 10:a, 11:r, 12:e, 13: , 14:i, 15:n, 
   
sentence = "the ducks are in a pond"
sample(sentence)
```

7. Iterate over a string, split it, and return each word along with its index using range(len())
```
def sample(sentence):
    
    words = sentence.split()
    
    for i in range(len(words)):
        print(f"{i}:{words[i]}", end=', ') // 0:the, 1:ducks, 2:are, 3:in, 4:a, 5:pond,
   
sentence = "the ducks are in a pond"
sample(sentence)
```

8. Iterate over a string using enumerate and print the word along with its index
```
def sample(sentence):
    
    words = sentence.split()
    
    for key, value in enumerate(words):
        print(f"{key}:{value}") // 0:the, 1:ducks, 2:are, 3:in, 4:a, 5:pond,
   
sentence = "the ducks are in a pond"
sample(sentence)
```
