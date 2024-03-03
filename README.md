# CS253_Assignment_1_Krutuparna_Paranjape

The assignment implements a Car Rental System in C++ using object oriented programming paradigms. The code is present in main.cpp. There are 3 kinds of users and each of them have different functionalities and specifications. They are outlined in the Problem Statement. All functionalities of the statement have been implemented acccordingly. 

- [Problem Statement](https://github.com/Rutuparn9/CS253_Assignment_1_Krutuparna_Paranjape/blob/main/Problem_Statement.pdf)

Database management has been done through c++ file handling.There are 3 csv files that serve as databases:

- [all_users_data.csv](https://github.com/Rutuparn9/CS253_Assignment_1_Krutuparna_Paranjape/blob/main/all_users_data.csv) stores details of all users [name,id,password,user_type,user_record]. The ```user_type``` is '1' for Customer, '2' for Employee and '3' for Manager. 
- [all_cars_data.csv](https://github.com/Rutuparn9/CS253_Assignment_1_Krutuparna_Paranjape/blob/main/all_cars_data.csv) stores the details of all cars in the format: [model_name,manufacturer,condition,serial_number, is_rented].```Codition``` stores the fields : 'new' and 'used'. The ```is_issued``` field is '1' if the car has been rented and zero otherwise. 
- [rented_cars_data.csv](https://github.com/Rutuparn9/CS253_Assignment_1_Krutuparna_Paranjape/blob/main/rented_cars_data.csv) stores details of all rented cars in the format :  [user id,model,serail_number, timestamp]. The ```user id``` is the id of the user who rented the car and ```timestamp``` stores the time when the user rented it.

To run the system, go to the directory where this repository is stored and type the following commands in the console:
```
g++ main.cpp -o main
.\main
```
The system will run on the console. 

__Assumptions__ : 
1) Every car is assumed to have been rented for 2 day.
2) Fine of Rs500 is calculated everyday post the due date.This fine is additional to the rental fee.
3) Rental fee of every car is Rs 1000 / day.Employees can avail a 15% discount on this fee.
4) Every customer and employee is assigned customer and employee record respectively.They can't rent cars more than their customer/employee record socres.
5) Whenver a new customer/employee is added, he/she is assigned an avg customer/employee record.

