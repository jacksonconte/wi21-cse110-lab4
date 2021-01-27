# Debugging
The bug was due to a concatenation of strings with the "+" operator rather than addition of numbers. This is because num1 and num2 are string inputs, so I would fix the bug by passing each of them through the Number() explicit conversion operation. (Screenshots included in repo)
