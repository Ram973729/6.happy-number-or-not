# 6.happy-number-or-not
def happynum(n):
    while(n!=0):
        b=0
        while(n!=0):
            a=n%10
            b=b+(a*a)
            n=n//10
        if b==1:
            return True
            break 
        elif b==2 or b==3 or b==4 or b==5 or b==6 or b==7 or b==8 or b==9:
            return False
            break
        n=b
n=int(input('Enter any number:'))
if(happynum(n)):
    print('Happy Number')
else:
    print('Not a Happy Number')
