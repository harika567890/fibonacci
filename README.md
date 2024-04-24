# fibonacci
def fibonacci_imitation(n):
    # Starting values
    a1, a2 = 1, 2
    if n == 1:
        return a1
    elif n == 2:
        return a2
    else:
        for i in range(3, n+1):
            a3 = a1 + a2 - 1
            a1, a2 = a2, a3
        return a3

# Calculate the 42nd term
fibonacci_42 = fibonacci_imitation(42)
print(fibonacci_42)
