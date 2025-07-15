# project-of-check-valid-Email-in-python



email=input("Enter the Email=")
k=0
j=0
d=0
if len(email)>=6:
    if email[0].isalpha():
        if ("@" in email) and (email.count("@")==1):
            if (email[-3]==".")^(email[-4]=="."):
                for i in email:
                    if i==i.isspace():
                        k = 1
                    elif i.isalpha():
                        if i==i.upper():
                            j=1

                    elif i.isdigit():
                        continue
                    elif i == "." or i == "_" or i == "@":
                        continue
                    else:
                        d = 1

                if k == 1 or j == 1 or d == 1:
                    print("Wrong email (rule 5)")
            else:
                print("wrong Email for . no (4)")
        else:
            print("wong Email for the @  no (3)")
    else:
        print("wrong email  for the alpha no (2)")
else:

