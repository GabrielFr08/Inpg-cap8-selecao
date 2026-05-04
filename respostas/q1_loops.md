a. Java
int k = (j + 13) / 27;
while (k <= 10) {
    k++;
    i = 3 * k - 1;
}

b. Python
k = (j + 13) // 27
while k <= 10:
    k += 1
    i = 3 * k - 1

c. Haskell
loop k i = if k > 10 then (k, i) else loop (k + 1) (3 * (k + 1) - 1)

d. Swift
var k = (j + 13) / 27
while k <= 10 {
    k += 1
    i = 3 * k - 1
}

Discussão: 
Para este código, o Python ganha disparado na facilidade de escrita e na legibilidade. A sintaxe é muito direta e a falta de chaves deixa o visual bem mais limpo. Java e Swift são bons, mas a verbosidade acaba cansando um pouco mais na hora de digitar.
