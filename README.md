def taken_name(surname_husband, surname_wife):

    
    for ch in range(0,len(surname_wife)):
        if surname_wife[ch] =="-":
            x = [ch]
            for ch in range(x,len(surname_wife)):
                if surname_husband in surname_wife:
                    return True
                else:
                    return False
        else:
            if surname_husband in surname_wife:
                return True
            else:
                return False
        

name_men = input ("Enter the name of husband: ")
name_woman = input ("Enter the name of wife: ")

print("Are Thay Family:",taken_name(name_men,name_woman))
