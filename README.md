# string-problem-statements
string problem statements with solutions
Write a Python function to create the HTML string with tags around the word(s).
def add_tags(tag, word):
    return "<%s>%s</%s>" % (tag, word, tag)
print(add_tags('i', 'Python'))
print(add_tags('b', 'Python Tutorial'))


Write a Python function to insert a string in the middle of a string.
s1='geekforgeeks is for geeks'
s2='Good'
temp=s1.split()
ln=len(temp)//2
def st(s1,s2):
    return ' '.join(temp[:ln]+[s2]+temp[ln:])
st(s1,s2)

.Write a Python function that accepts a string and calculate the number of upper case letters and lower case letters.
def cal(st):
    c=0
    x=0
    for i in st:
        if i.isupper():
            c+=1
        elif i.islower():
            x+=1
       
    print('number of upper case letters of',st,c ,'and number of upper case letters of',st,x)
cal('Pooja Tibile')

Write a Python function to check whether a string is a pangram or not. Go to the editor
Note : Pangrams are words or sentences containing every letter of the alphabet at least once.
For example : "The quick brown fox jumps over the lazy dog"
def pangram(str):
    alphabet='abcdefghijklmnopqrstuvwxyz'
    for i in alphabet:
        if i not in str.lower():
            return 'not pangram'
    return 'pangram'
print(pangram("The quick brown fox jumps over the lazy dog"))
