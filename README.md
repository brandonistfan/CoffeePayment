# CoffeePayment

## Introduction
The employees at Bertram Labs have a daily coffee run that has created a logistical challenge. Bob, Jeremy, and 5 other coworkers enjoy walking to the local coffee shop every day after lunch to grab their favorite drinks—a cappuccino for Bob, black coffee for Jeremy, and varying choices for the others. To streamline the checkout process, one employee pays for the entire order each day.

The trouble is, with different drink choices and prices, the employees have a hard time keeping track of whose turn it is to pay. This can lead to confusion, frustration, and a lack of fairness if some employees end up paying more than others over time.

To address this, I have developed a software program to evenly distribute the responsibility of paying for the coffee order. By randomly choosing a new designated payer each day and keeping track of drink costs and history, the program aims to bring simplicity and fairness to the daily coffee run.

The core goal is to remove the mental burden from the employees so they can focus on enjoying their afternoon coffee break. This program tracks spend history, assigns a daily payer, and ensures a fair rotation over time, regardless of drink price variances.

## Installation 
To install CoffeePayment, please follow these steps:

- Ensure Java is installed on your system. CoffeePayment requires Java 8 or newer. Verify your Java version by executing java -version in your command prompt or terminal.
- Download the CoffeePayment-1.0-SNAPSHOT.jar file from the project's release section.
- Save the JAR file in your preferred directory.

## Usage

Running CoffeePayment is straightforward. Open a terminal or command prompt, use the Gradle Wrapper to build the project.
- On Unix operating systems, run:
  - ./gradlew build
- On Windows, run:
  - .\gradlew.bat build

Then, navigate to the folder containing CoffeePayment-1.0-SNAPSHOT.jar, and run:  

- java -jar CoffeePayment-1.0-SNAPSHOT.jar  

The application will guide you through the process, from selecting beverages to determining who should pay for the day's coffee order, ensuring a fair rotation based on the cost of the beverages.

## Assumptions
In developing a solution for the Bertram Labs coffee run, several assumptions have been made:
- Coworker attendance: It is assumed that not all coworkers will participate in the coffee run each day. Some employees may be out of the office for meetings, time-off, etc. The solution is designed to handle fluctuating daily attendance.
- New and departing coworkers: It is expected that the makeup of the group participating in the coffee run will change over time as new employees join Bertram Labs and others potentially leave. The solution can dynamically adjust for any changes to the group.
- Drink preference changes: While each current employee has a regular drink order, it is possible they may decide to order something new on occasion. The randomness and flexibility built into the solution allows it to easily accommodate changes in drink selections.
