# CS253_Assignment_1_Krutuparna_Paranjape

The assignment implements a car rental system in C++ using object oriented programming paradigms. The code is present in main.cpp. There are 3 kinds of users and each of them have different functionalities and specifications. They are outlined in the Problem Statement. All functionalities of the statement have been implemented acccordingly. There are 3 csv files which serve as databases.

[problem Statement]()


- [all_users_data.csv]() stores [name,id,password,type of user,user_record]. The type of user '1' is for customer, '2' is for employee and '3' is for manager. 
- [all_cars_data.csv]() stores the details of all cars in the format: [model_name,manufacturer,condition,serial_number, is_rented].```Codition``` stores the fields : 'new' and 'used'. The ```is_issued``` field is '1' if the book has been issued by a user and zero otherwise. One row in the file stores the data of one book.
- [rented_cars_data.csv]() stores details of all rented cars in the format :  [user id,model,serail_number, timestamp]. The ```user id``` is the id of the user who rented the car and ```timestamp``` stores the time when the user issued it.

To run the system, go to the directory where this repo is stored and type the following commands in the console:
```
g++ main.cpp -o main
.\main
```
The system will run on the console. 
