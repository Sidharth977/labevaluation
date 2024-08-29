def balanced_diet(sport):
    if sport=="football":
        return "eat fruits and protien based food"
    if sport=="cricket":
        return "eat good carbs and milk"
    else:
        return "eat carbs vitamins and cereals"    
dict2={}
n=int(input("enter the number of students ="))
for i in range(0,n,1):
    name=input("enter the name of the student")
    clas=int(input("enter the class of the student"))
    height=int(input("enter the height of the student"))
    weight=int(input("enter the weightof the student"))
    perfferd_sport=input("enter the prefferd_sport")
    dict2.update({"name":name})
    dict2.update({"class":clas})
    dict2.update({"height":height})
    dict2.update({"weight":weight})
    dict2.update({"prefferd_sport":perfferd_sport})
    print(dict2)
for i in dict2:
    if(i=="prefferd_sport"):
        result=balanced_diet(i)
        print(result)
