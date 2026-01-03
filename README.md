 Project Overview

MediTrack is a console-based Java application designed to manage doctors, patients, appointments, and billing in a medical environment.
The project demonstrates core Java concepts, Object-Oriented Programming (OOP) principles, JVM understanding, and design patterns, as required by the assignment specification.

The application follows a layered architecture using services, entities, utilities, interfaces, and enums, and provides a menu-driven user interface for interaction.

 Features Implemented
 Core Functionalities

CRUD operations for Doctors and Patients

Appointment management:

Create appointment

View appointments

Cancel appointment using AppointmentStatus enum

Billing system with tax calculation

Menu-driven console UI using Scanner

 Object-Oriented Programming Concepts

Encapsulation: Private fields with controlled access

Inheritance: Person → Doctor, Patient

Polymorphism:

Method overriding

Interface-based dynamic binding

Abstraction:

Abstract classes

Interfaces with default methods

 Advanced Java Concepts

Enums: Specialization, AppointmentStatus

Immutable Class: BillSummary

Deep Copy: Cloneable implementation for Patient and Appointment

Generics: DataStore<T> for reusable storage

Collections: ArrayList, HashMap

Static blocks & variables

Exception handling

 Design Patterns Used

Strategy Pattern

BillingStrategy interface

StandardBillingStrategy, InsuranceBillingStrategy

Singleton Pattern

IdGenerator for unique ID creation

 Project Structure
com.airtribe.meditrack
│
├── Main.java
│
├── constants
│   └── Constants.java
│
├── entity
│   ├── Person.java
│   ├── Doctor.java
│   ├── Patient.java
│   ├── Appointment.java
│   ├── Bill.java
│   └── BillSummary.java
│
├── enums
│   ├── Specialization.java
│   └── AppointmentStatus.java
│
├── interfaces
│   ├── Payable.java
│   ├── Searchable.java
│   └── BillingStrategy.java
│
├── service
│   ├── DoctorService.java
│   ├── PatientService.java
│   ├── AppointmentService.java
│   ├── StandardBillingStrategy.java
│   └── InsuranceBillingStrategy.java
│
├── util
│   ├── Validator.java
│   ├── DateUtil.java
│   ├── CSVUtil.java
│   ├── IdGenerator.java
│   └── DataStore.java
│
├── exception
│   ├── AppointmentNotFoundException.java
│   └── InvalidDataException.java
│
├── test
│   └── TestRunner.java
│
└── docs
    ├── Setup_Instructions.md
    └── JVM_Report.md

 Technologies Used

Java (JDK 8+)

Eclipse / IntelliJ IDEA

Java Collections Framework

Java Streams & Lambdas (bonus)
