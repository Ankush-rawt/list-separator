# list-separator
A simple  program that separates list of even and odd numbers from a user-input  using a function. Demonstrates basic list operations, conditionals, and function return values.
def seprate(num):
    even_num=[]
    odd_num=[]
    for n in num:
        if n%2==0:
            even_num.append(n)
        else:
            odd_num.append(n)  
    return even_num,odd_num

num_list=input("enter list : ").split()
real_list =[int(n) for n in num_list]

even_num,odd_num= seprate(real_list)
print ("even : ",even_num)
print ("odd : ",odd_num)
