a. C
switch (k) {
    case 1: case 2: j = 2 * k - 1; break;
    case 3: case 5: j = 3 * k + 1; break;
    case 4: j = 4 * k - j; break;
    case 6: case 7: case 8: j = k - 2; break;
}

b. Ruby
case k
when 1, 2 then j = 2 * k - 1
when 3, 5 then j = 3 * k + 1
when 4 then j = 4 * k - j
when 6..8 then j = k - 2
end

c. Erlang
J = case K of
    1 -> 2 * K - 1;
    2 -> 2 * K - 1;
    3 -> 3 * K + 1;
    5 -> 3 * K + 1;
    4 -> 4 * K - J_old;
    _ when K >= 6, K =< 8 -> K - 2
end.

Discussão:
A vantagem do Ruby aqui é a flexibilidade de usar intervalos como '6..8', o que economiza várias linhas de código. O C funciona bem, mas o excesso de 'breaks' torna o código mais propenso a erros de lógica se a gente esquecer um deles.
