
# Instructions

Here you can find all necessary flows to implement Datebase.

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

The flow update JDS Token Template is used to update the JDS Tokens. This flow is periodicly runs by a scheduler.

<img width="989" alt="image" src="https://github.com/user-attachments/assets/912c324e-3782-4f58-8a2e-50b4640b149f" />

In these flow also the Client ID and Secret are defined as variables, so we can use the token refresh procedure.

After token refresh we update the profile with the new access and refresh token.


