Linguagem 1: Java
int j = -3;
boolean stop = false;
for (int i = 0; i < 3 && !stop; i++) {
    int val = j + 2;
    if (val == 3 || val == 2) j--;
    else if (val == 0) j += 2;
    else j = 0;
    if (j > 0) stop = true;
    else j = 3 - i;
}

Linguagem 2: Python
j = -3
for i in range(3):
    val = j + 2
    if val in [2, 3]: j -= 1
    elif val == 0: j += 2
    else: j = 0
    if j > 0: break
    j = 3 - i

Linguagem 3: C++
int j = -3;
for (int i = 0; i < 3; i++) {
    int val = j + 2;
    if (val == 2 || val == 3) j--;
    else if (val == 0) j += 2;
    else j = 0;
    if (j <= 0) j = 3 - i;
    else i = 3;
}
