class terminal():
    balans=1000
    def __init__ (self):
        print("Bankomatning hozirgi balansi($):")
    def funcq(self,summ):
        self.summ=summ
        return self.balans+summ
    def func(self,summ):
        self.summ=summ
        return self.balans-summ
k=input("Agar pull yechmoqchi bo'lsingiz 1 ni, pull tushirmoqchi bo'lsangiz 0 ni kiriting: ") 
su=int(input("Pull miqdorini kiriting($): "))
my_r=terminal()
if k=="0":
    my=my_r.funcq(su)
elif k=="1":
    my=my_r.func(su)
print(my)
