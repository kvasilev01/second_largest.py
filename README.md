>>> def second_largest(numbers):

    first, second = False, False
    
    for n in numbers:
    
        if n > first:
        
            first, second = n, first
            
        elif first > n > second:
        
            second = n
            
    return second
    
>>> second_largest([5, 6])

5

>>> second_largest([5, 5])

False

>>> second_largest([1])

False
>>> 
