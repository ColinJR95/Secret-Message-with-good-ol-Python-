# Secret-Message-with-good-ol-Python-

import os 
def rename_files(): 
    file_list = os.listdir(r"C:\Users\houseguest\Desktop\prank")
    print file_list

    
    os.chdir(r"C:\Users\houseguest\Desktop\prank")

    for file_name in file_list:
        os.rename(file_name,file_name.translate(None,"0123456789"))
        saved_path = os.getcwd()
        print ("Current Working Directory is " + saved_path)
        os.chdir(saved_path)      
rename_files()






