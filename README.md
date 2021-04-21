# Project billing kata

This exercise is inspired by an actual software tool that we are developing internally at Lean Mind. 

## The problem

The way we charge our customers is mostly through time and materials, basically the amount of hours spent by developers. For each project, there could be one or several contracts, although only one contract is valid at at time. A project could start off as soon as the contract is signed off with an initial duration of N months and certain conditions - rates, payment dates.... After the contract is finished a new one could be signed off so that the project could go on for another bunch of months and perhaps different terms and conditions - different rates perhaps. 

During the length of a contract the number of developers working on a project don't usually change although they could. The amount of hours spent may certainly fluctuate as some people could get sick or go on vacation. We assume there is another piece of software in which people register the amount of hours worked per day. The rates per hour and seniority level don't change. The seniority level of a developer doesn't change during the duration of the contract. 

At the end of each worked month, the software is used to create an invoice with the **total cost of development (hours per person) plus fees, in case certain fees apply**. 

The goal of the kata is to think of a design that supports the calcultation of the monthly invoice. To simplify the exercise, you could think of a method or function that returns **an amount of money**. The artifact would need to be given a month, a year, a contract and the records of worked hours per developer. You get to decide how would you like that information to be found in the data source. 

Contract example:

    - Starts on Date A
    - Ends on Date B
    - Two senior developers at X €/hour will work for 35 hours a week.
    - Three mid developers at Y €/hour will work for 35 hours a week.
    - One junior developer at Z €/hour will work for 35 hours a week.

You could come up with database tables although the more interesting part of the kata is the software design, the source code in your preferred programming language. Do not design stored procedures, make sure the login is in the code, not the database. The kata could be more valuable if you try different programming paradigms and compare them. As usual katas are useful when practices many times with a variety of approaches.  

## Possible dojo structure

 * The facilitator spends 15 minutes introducing the problem to the group. 
 * Each individual groups on a design alone - 20 minutes.
 * In small groups of three or four people (or pairs), the designs are shared and discussed - 30 minutes
 * One of the chosen designs is written in the form of source code - 10 minutes. 
 * The whould group get together and the code is shared with all of them.


