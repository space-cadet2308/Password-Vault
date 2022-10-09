import random
import pickle
from tkinter import Y
info = {}
red = {}
will = input("Do you want to enter your own Password(y/n):")
if "y" in will:
    f1 = open("saved.pass", "ab")
    app_name = input("Name of the application:")
    acc_name = input("Enter name of User_id:")
    acc_pass = (input("Enter your password:"))
    red[app_name] = acc_name + "-->" + acc_pass
    with open("saved.pass", "ab") as file1:
        pickle.dump(red, file1)
    print("Password is saved")
    f1.close()
elif "n" in will:
    alpha = "ABCDEFGHIJKLMNOPQRSTUVWXYZ" \
            "abcdefghijklmnopqrstuvwxyz1234567890!@#$%^&*()_+"
    len_pass = int(input("No. of digits in password :"))
    file = open("saved.pass", "ab")
    password = "".join(random.sample(alpha, len_pass))
    print(password)
    ans = input("Do you want to keep this password(y/n) : ")
    if "y" in ans:
        app_name = input("Name of the application:")
        acc_name = input("Enter name of User_name:")
        info[app_name] = acc_name + "-->" + password
        with open("saved.pass", "ab") as file:
            pickle.dump(info, file)
        print("Password saved")
    else:
        print("Password is not saved")

        x = input("Want to try again?(y/n)")
        if "y" in x:
            file = open("saved.pass", "ab")
            password = "".join(random.sample(alpha, len_pass))
            print(password)
            ans = input("Do you want to keep this password(y/n) : ")
            if "y" in ans:
                app_name = input("Name of the application:")
                acc_name = input("Enter name of User_name:")
                info[app_name] = acc_name, password
                with open("saved.pass", "ab") as file:
                    pickle.dump(info, file)
                print("Password is saved")
            else:
                print("Thank you :)")
else:
    print("Please input a correct response")
print("Thank you :)")
