# pythontip
pythontip
def closest_power(base,n):
    exp=0
    while True:
        if base**exp>=n:
            break
        exp+=1
    if abs(n-base**exp)>=abs(n-base**(exp-1)):
        return exp-1
    elif abs(n-base**exp)<abs(n-base**(exp-1)):
        return exp
