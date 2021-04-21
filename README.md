# Project billing kata

This exercise is inspired by an actual software tool that we are developing internally at Lean Mind. 

The way we charge our customers is mostly through time and materials, basically the amount of hours spent by developers. For each project, there could be one or several contracts, although only one contract is valid at at time. A project could start off as soon as the contract is signed off with an initial duration of N months and certain conditions - rates, payment dates.... After the contract is finished a new one could be signed off so that the project could go on for another bunch of months and perhaps different terms and conditions - different rates perhaps. 

During the length of a contract the number of developers working on a project don't usually change although they could. The amount of hours spent may certainly fluctuate as some people could get sick or go on vacation. We assume there is another piece of software in which people register the amount of hours worked per day. The rates per hour and seniority level don't change. The seniority level of a developer doesn't change during the duration of the contract. 

At the end of each worked month, the software is used to create an invoice with the total cost of development (hours per person) plus fees, in case certain fees apply. 

The goal of the kata is to think of a design that supports the calcultation of the monthly invoice. To simplify the exercise, you could think of a method or function that returns an amount of money. The artifact would need to be given a month, a year, a contract and the records of worked hours per developer. 

Contract example:

    - Starts on Date A
    - Ends on Date B
    - Two senior developers at X €/hour will work for 35 hours a week.
    - Three mid developers at Y €/hour will work for 35 hours a week.
    - One junior developer at Z €/hour will work for 35 hours a week.


