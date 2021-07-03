# -args-and-kwargs
#here is code for args and **kwargs
# def function1(a,b,c,d):
#     print(a,b,c,d)
# function1("awanish","akash","sonam",'shiva')

def funargs(ch,*awa):
    print(ch)
    for i in awa:
        print(i)
    print(*awa)
har=["sonam","riddhi","soni","babta","kamal"]
d="Hello , I am here"
funargs(d,*har)

def funargs(ch,*awa,**kwargs):
    print(ch)
    for i in awa:
        print(i)
    for key,value in kwargs.items():
        print(key,"is a",value)
    print(*awa)
har=["sonam","riddhi","soni","babta","kamal"]
mema={"awanish":"student","aksh":"dancer","sonam":"actor"}
d="Hello , I am here"
funargs(d,*har,**mema)
