# file-handling
wk4



#create a file  called input.txt
#with the following content
# 1 Nodejs is best for backend 
# 2 Django is best for backend
# 3 React is best for frontend
# 4 PHP is good  for backend
# 5 javascript is good for frontend

with open('input.txt', 'w') as f:
    f.write("1 Nodejs is best for backend\n2 Django is best for backend\n3 React is best for frontend\n4 PHP is good  for backend\n5 javascript is good for frontend\n")

with open('input.txt', 'r') as f:
    data = f.read()
    print(data)
try:
    with open("input.txt", "r") as file:
        lines = file.readlines()
        for line in lines:
            if "upend" in line:
                print(line)
except FileNotFoundError:
    print("File not found. Please check the file path.")
except Exception as e:
    print(f"An error occurred: {e}")

