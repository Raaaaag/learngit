Git is a distributed version control system.
Git is free software distributed under the GPL.
Git has a mutable index called stage.
Git tracks changes of files.
My stupid boss prefers SVN.

xncopy = x_n
s = 0
for x, y in xncopy:
    s += x
x_ave = s / 10000
s1 = 0
s2 = 0
for t in range(10000):
    for n in range(1, 10000-t):
        s1 += (xncopy[n+t][0] - x_ave) * (xncopy[n][0] - x_ave)
        s2 += xncopy[n][0] * xncopy[n][0]
    c_t = s1 / s2
    print(s1, s2, c_t, t)
    if c_t == 0:
        rs = t
        break