### 🧾 User Defined Data Types — Nested Structures in C

## 🎯 AIM
To create a C program that prints a person's details like name, age, and address using nested structures.

## 📚 THEORY
A structure in C is a user-defined data type that allows grouping variables of different types under a single name.
A nested structure means one structure is declared inside another, allowing logical grouping of related information.

## 🔁 ALGORITHM
Define a structure address with fields:

houseno (integer)

street (string)

stateno (integer)

Define a structure person with fields:

name (string)

age (integer)

adr (structure of type address)

Create a variable of type person.

Accept user input for all the fields.

Display the details using printf.

## 🧾 STRUCTURE DEFINITION
```
struct address {
    int houseno;
    char street[20];
    int stateno;
};

struct person {
    char name[30];
    int age;
    struct address adr; // Nested structure
};
```
## 🖥️ PROGRAM
```
#include <stdio.h>

/* Declaration of structure */
struct address {
    int houseno;
    char street[20];
    int stateno;
};

/* Nested structure */
struct person {
    char name[30];
    int age;
    struct address adr;
};

int main() {
```
#include<stdio.h>

/* Declaration of structure */
struct address
{
 int houseno;
 char street[20];
 int stateno;
};
struct person
{
 char name[30];
 int age;

};

int main()
{
 struct person stud;
 struct address add;
 
 scanf("%s %d",stud.name, &stud.age);
 scanf("%s %d %d",add.street,&add.houseno,&add.stateno);
 
 printf("Name: %s Roll: %d\n", stud.name, stud.age);
 printf("Address:%s, House no. %d, state: %d",add.street, add.houseno, add.stateno);
 
 return 0;
}
```

## 🧪 SAMPLE INPUT & OUTPUT
![alt text](image.png)


## ✅ RESULT
Hence, the C program to print the person details like name, age, and address using nested structures is successfully executed.