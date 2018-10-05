# Student-Comments
#Goal is to take students names and attach comment to each name according to grade. The comments must not be use twice for the #same student and not used twice in the same class. 

from string import digits

lines = []
while True:
    line = input()
    if line:
        lines.append(line)
    else:
        break
text = "".join(lines)

print (text)

s = (text)
remove_digits = str.maketrans('', '', digits)
res = s.translate(remove_digits)


print(res)

w = (res)


remove_dots = str.maketrans('', '', "....")
no_dot = w.translate(remove_dots)

print(no_dot)


#Seperating

x = 0

phrase = "stuPidEDyouareSOdumBs"
names = []
for l in phrase:
    names.append(l)
    if l.isupper():
        x+=1
        if x%3 == 0:
            names_list = "".join(names)

            remove_stuff = str.maketrans('', '', "' , ")
            no_stuff = names_list.translate(remove_stuff)

            print(no_stuff + " good job")
            names = [""]


