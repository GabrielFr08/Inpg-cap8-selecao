1. C++
for (int i = 0, j = 17; i < n; i++, j--) sum += i * j + 3;

2. JavaScript
for (let i = 0, j = 17; i < n; i++, j--) sum += i * j + 3;

3. Python
j = 17
for i in range(n):
    sum += i * j + 3
    j -= 1

4. Go
for i, j := 0, 17; i < n; i, j = i+1, j-1 {
    sum += i * j + 3
}

5. PHP
for ($i = 0, $j = 17; $i < $n; $i++, $j--) {
    $sum += $i * $j + 3;
}
