
# Instructions

Here you can find all necessary flows to implement Database.

## Database overview

In these folder we describe who you can manage the database.

In the first step we need a database with two tables and the following attributes.

Table: account  
Attributes:  customerEmail,mainTel,secondaryTel,ccTel,customerName,contacted

Table: orders  
Attributes:  orderID,productID,productName,price,customerEmail,deliveryDate,status

## manage Account

When a account is created on Website the flow Account Management Template is executed.

The flow is creating or deleting a account in the database.

<img width="1378" alt="image" src="https://github.com/user-attachments/assets/c15d5c03-10b5-4041-be74-f6f66c9f6f30" />

Also a person in JDS is generated. Here is an example of that.

<img width="933" alt="image" src="https://github.com/user-attachments/assets/51612772-8ee8-4a1d-bf7f-7863e60be576" />

## manage orders

When a order is created on Website the flow Website Order Confirmation Template is executed.

<img width="1378" alt="image" src="https://github.com/user-attachments/assets/e2441b35-d380-4d78-9013-b1fd828a0fbe" />

The flow is generating the delivery date and add the order to database. After that an confirmation mail is send to the Email address of account. Also a subflow to 
inject JDS entry for the order is called.

<img width="720" alt="image" src="https://github.com/user-attachments/assets/7310b663-ace6-40d4-953b-52c907c68998" />

Here is an example for JDS injecting.

<img width="927" alt="image" src="https://github.com/user-attachments/assets/35dec89c-5939-4e77-803d-03d08bc521ec" />

## cancel order

