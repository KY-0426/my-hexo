python ：已知两边及其夹角球第三边

import math
x=input('输入两边长及夹角（度）:')#输入时候使用空格分隔3个值
a,b,theta=map(float,x.split())#序列解包，split()方法用于切分字符串
c=math.sqrt(a**2+b**2-2*a*b*math.cos(theta*math.pi/180))
                    #cos()参数为弧度
print('c=',c)

