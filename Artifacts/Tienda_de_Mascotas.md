# Scales Pet Shop CRUD
Universidad Autonoma de Ciudad Juarez
Instituto de Ingeneria y Tecnologia
Ingeneria en Software
Hector Gerardo Sanchez Quiroga 
169840
Desarollo de requisitos de software
# Introduction
The next section will talk about the general idea of the project, it will talk about the purpose, scope, definitions, and references. 

## Purpose
There is a need to start developing programs. That work and are in need in the real world. Here we have a problematic. For the Pet Store, that needs a CRUD to be developed.

## Scope

"Pets Store Management System " will be an application designed to be developed in Java with a database connection, where you can create, read, update and delete the animals that are currently in the pet-store. The data that will be store about the pets will be: IdPet, NamePet, WeightPet, PetBreed, PetOwner, and different checks for the services and status of the pet. There will be restrictions on who can access the information, in example a Cashier can not change the attribute of ate.  
The users that can consult the system are the Cashier, the Stylist, the Stocker, and the Pet Shop Assistant.
There are different users with different authority in the system, to which, not all users can access the data in the same way.
Although the project can be managed and designed to be commercialized, it will be more focused on an academic purpose.

## Definitions, acronyms, and abbreviations
| Acronyms, and abbreviations | Definitions                                                                                                                                                                       |
|-----------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Pet_ID                      | This attribute will be the Id that the Pet will receive when it gets registered in the store. The Id will help the System to distinguish these pet. And make a Particular Object. |
| Pet_Name                    | This attribute will give the name of the pet.                                                                                                                                     |
| Pet_Weight                  | This attribute will give the weight of the pet.                                                                                                                                   |
| Pet_Breed                   | This attribute will give the breed of the pet.                                                                                                                                    |
| Pet_Owner                   | This attribute will give the name of the pet Owner.                                                                                                                               |
| CleanStatus                 | This attribute will give the user to known if an animal has been cleaned, or hasn't.                                                                                              |
| CheckStatus                 | This attribute will give the user information of the pet, if it has been checked, sick, or is healthy.                                                                            |

## References

# Overall Description

The next section will give an overview of the system. The section will explain how the system interacts with other systems. These Systems can be a database where the data will be accesed. 
## Product Perspective
The system consists of a CRUD the diferrent employees can Create, Read, Update, and Delete the data.:
*Create:
The system consists of an application for consultation and modification of data, therefore it is divided into 
  *The first part is the area of the search. Here the client can search and see the information of the product.
  *The application needs a constant communication with the database to retrieve the information in real time and thus show the current status of each pet, such as type, breed, age, and status. The status means if the Pet is ready to leave, or is still in care. It can be a cleaning procedure.(These status is only valid in pets, the other products can't have this status)


## Product functions

The main function of the system is to provide information to the user about the pet status, and when the pet is ready to go.
Thus making an application for the management of pets in a Pets store.

## User characteristics

| Actor              | Role                                                                                                                                                                                                                                                                                               |
|--------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Cashier            | The role for the cashier will be to Collect the payment, Give change to the client, Charge the customer, and finally give the product to the client.                                                                                                                                               |
| Pet Shop Assistant | The role for the Pet Shop Assistant will be to Feed Pets, Clean the Cages when they are dirty (These includes fish tanks), Advise the customer in which pet to buy, Check Fish Tanks, and Check the animal in the Physical Check-Up                                                                |
| Stylist            | The role of the Stylist will be to Cut the pet's fur, Brush the fur, Wash the Pet (In these process we make a sub-process of checking the anal glandules), Dry the pet, and finally cut the Pet's nails. The owner can also decide to add a Accesory, these increases the cost but it's an option. |
| Client             | His role is to buy products, or leave the pet for it to be checked or clean.                                                                                                                                                                                                                       |
| Pet                | His role is to be checked and cleaned.                                                                                                                                                                                                                                                             |


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
### FR1: Change Status for VET:
Desc: The vet can change the status of the Check-UP status
### FR2: Change Status for Stylist:
Desc: The Stylist can change the Status of the Clean Status
### FR3: Receive notifications for Re-stock or help
Desc: The Employee must receive a notification when an animal needs to be feed
### FR4: Search the product
Desc: The client can search a product and see the information about that product.



# BPM
![BPM](https://github.com/RequirementEngineering/ch-re-169840HectorSanchez/blob/master/Artifacts/PetStor_BPD.jpg?raw=true "BPM")

# Elicitation;
 There was an Elicitation process with Valeria Perez:
 Valeria: The first thing they do, will be bring your dog or cat to the Petstore. Inside the Petstore you go to left side of the entrance, there you will see a cashier. In the cashier, they will register your dog, and ask what will you like to do. It can be a normal check-up, or a Check-Up with bath included. (She said that the reason they dont give a Bath only is because they need to confirm that the dog or cat is in healthy conditions. If it isn't they will first try to eliminate the "disease").
 
 The process in which a Petshop does a check-up, is by: A physical examination:
 1. Check Weight, Body Temperature
 2. Ask questions about the pet, these questions are: Diet, Exercise, Secretion, livehood.
 3. Check Hair, Skin, Eyes, Ears
 4. Check breathing, and teeth.
 5. Measure Heart Rate
 6. Feel legs, and abdomen. (Feeling these areas can detect pain or discomfort)
 
 After, the pet have had the checkup, then the Stylist proccess continues the process is:
 1. Cut hair
 2. Brush hair
 3. Wash
 4. Drying
 5. Rebrush
 6. Trim Nails
 7. Extra: You can add accesories to the dog ex: Ribbon, etc.
 
 The problem is mainly in the area of the pets, they only use paper to keep information about the animals. It can be useful to have a program that retains the information of the pets that are currently in the cleaning area or the checkup. The use of paper can complicate the process, because they often forget to write on the paper, and the information in the paper is not certain. These can make them lose money.
