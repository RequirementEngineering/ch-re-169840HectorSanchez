# Scales Pet Shop CRUD
# Introduction
The next section will talk about the general idea of the project, it will talk about the purpose, scope, definitions, and references. 

## Purpose
There is a need to start developing programs. That work and are in need in the real world. Here we have a problematic. For the Pet Store, that needs a CRUD to be developed.

## Scope

"Pets Store Management System " will be an application designed to be developed in Java with a database connection, where you can create, read, update and delete products from a store. It will have as data: the name of the product, an ID and its price. Where the user will be able to consult said information. The products include pets, food, toys, collars, cat litter, cages, and aquariums. 
The users that can consult the system are the employeer, owner-administrator, and the client.

There are different users with different authority in the system, to which, not all users can access the data in the same way.

Although the project can be managed and designed to be commercialized, it will be more focused on an academic purpose.

## Definitions, acronyms, and abbreviations
Admin: Administrator
## References

# Overall Description

The next section will give an overview of the system. The section will explain how the system interacts with other systems. These Systems can be a database where the data will be accesed. 
## Product Perspective

The system consists of an application for consultation and modification of data, therefore it is divided into two parts:
  *The first part is the area of the search. Here the client can search and see the information of the product.
  *The application needs a constant communication with the database to retrieve the information in real time and thus show the current status of each pet, such as type, breed, age, and status. The status means if the Pet is ready to leave, or is still in care. It can be a cleaning procedure.(These status is only valid in pets, the other products can't have this status)


## Product functions

The main function of the system is to provide information to the user and the complete management of the system to the administrator. Thus making an application for the management of a Pets store.

## User characteristics
In these system, ther will be three types of users. The first type of user, is the client. 

| Actor         | Role                                                                                                                                                             |
|---------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Employee      | Can check if there is stock of the product, when a products needs stock, the employee will go and re-stock, see if a client needs help.|
| Administrator | He can access the products, and make internal changes to the products attributes. He can order the employee to re-stock.|
| Client        | Can search for a product, and see the description and attributes of the product. He can also save the products he wants in an wish-list.                                                                                                                                       |


![Use Case](https://github.com/RequirementEngineering/ch-re-169840HectorSanchez/blob/master/Artifacts/Pet%20Store%20Use%20Case.jpg?raw=true)
## Constraints
The different interfaces that are needed can become a restriction due to the difficulty of adapting. Since it opens a difference of navigation depending on the type of user.

The hardware can be an impediment due to the high cost it can generate for a petstore.

If you want the end user to search for the product, you need a more functional interface that is face-to-face / physical.
The product needs to be easy to use, and simple. As the clients and employees doesnt need a capacitation to start using it.
## Assumptions and dependencies
| Assumptions(AS) & Dependencies(DE) | Description                                                          |
|------------------------------------|----------------------------------------------------------------------|
| AS-1                               | The system will be used in a desktop.                                |
| AS-2                               | Only Employees can access the stock area of the software.            |
| AS-3                               | The clients can only search and find the attributes of the products. |
| DE-1                               | Needs a Computer, Internet-Connected, and Electricity to work        |
| DE-2                               | Needs a Database connection                                          |


# Specific requirements

## External interface Requirements
This section provides a detailed description of all inputs into and outputs from the system. It also gives a
description of the hardware, software and communication interfaces and provides basic prototypes of the
user interface.

## User Interface
The first instance when the user enters the program. He can see a screen where there is a search button and a text box where the user will insert the object's name. And click on search, the program will then send the user to screen where the products will appear.
If the user is an employee or administrator, he must sign into his account, the account type will be: ID-Scales@Scales.com Example.
After this, if he is an employee he can see in the system if a certain products needs re-stock, and he will be notified, this also happens if a client asks for help. 
In case of an administrator, he must sign into his account. Then in the system here, he can make changes to the diferrent products and order re-stocks to the employees. Here is where the CRUD comes, the administrator can Create, Read, Update, Delete.
## Hardware Interface
It doesn't have any designated hardware, but it can be used on PCs.
## Communications interfaces
The employee will be notified when he needs to make a re-stock.
# Functional requirements
### FR1: CRUD for Administrator:
Desc: The administrator can change, read, update or delete the different products. 
### FR2: Order re-stocks- Admin
Desc: The administrator can order to re-stock to a certain employee.
### FR3: Receive notifications for Re-stock or help
Desc: The Employee must receive a notification when he needs to re-stock
DEP: FR3, FR5
### FR4: Search the product
Desc: The client can search a product and see the information about that product.
### FR5: Send notification for help
Desc: Send a notification to an employee when a client needs help.
### FR6: Check for re-stock
Desc: The employee can check if there is a need for re-stock in any of the areas.

# Class Diagrams

# Elicitation
 There was an Elicitation process with Valeria Perez, the process in which a Petshop does a check-up, is by: A physical examination.
 1. Check Weight, Body Temperature
 2. Ask questions about the pet, these questions are: Diet, Exercise, Secretion, livehood.
 3. Check Hair, Skin, Eyes, Ears
 4. Check breathing, and teeth.
 5. Measure Heart Rate
 6. Feel legs, and abdomen. (Feeling these areas can detect pain or discomfort)
 
 After, the pet have had the checkup, then the Stylist proccess continues
