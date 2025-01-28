def repeat(s):
    freq = {}
    
    for char in s:
        freq[char] = freq.get(char, 0) + 1
    
    for char in s:
        if freq[char] == 1:
            return char
    
    return 'Not Found'
s = input("Enter a string: ")

result =repeat(s)
print(f"First non-repeating character: {result}")
