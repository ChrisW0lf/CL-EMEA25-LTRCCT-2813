
# Instructions

Here you can find all necessary flows to implement JDS.

## JDS  Flows
In these folder we describe who you can manage JDS Tokens.

For this we use the profile node integrated in Connect to store and update the tokens. The profile node is a database within connect.

## init Profile

with the create JDS Profile Template Flow we are creating a Profile with customer id 2025. 

<img width="529" alt="image" src="https://github.com/user-attachments/assets/5887c3bb-9b10-4d82-a819-ddcb05230bab" />

We also add the following values ​​to the individual variables: Name --> Accesstoken msisdn --> Refreshtoken

<img width="942" alt="image" src="https://github.com/user-attachments/assets/9521402f-5bdf-432d-bb34-0d58fdde7f25" />

Now the Profile with customerid 2025 holds both tokens.

## refresh Token

The flow update JDS Token Template is used to update the JDS Tokens. This flow is periodicly runs by a scheduler.

<img width="989" alt="image" src="https://github.com/user-attachments/assets/912c324e-3782-4f58-8a2e-50b4640b149f" />

In these flow also the Client ID and Secret are defined as variables, so we can use the token refresh procedure.

After token refresh we update the profile with the new access and refresh token.

