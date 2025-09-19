def factorial(n):
    """
    This function calculates the factorial of a non-negative integer.
    """
    if n < 0:
        return "Giai thừa không tồn tại cho số âm"
    elif n == 0:
        return 1
    else:
        result = 1
        for i in range(1, n + 1):
            result *= i
        return result

# Ví dụ sử dụng hàm
number = 5
print(f"Giai thừa của {number} là: {factorial(number)}")
