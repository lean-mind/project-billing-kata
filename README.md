# Project billing kata

This exercise is inspired by an actual software tool that we are developing internally at Lean Mind. 

The way we charge our customers is mostly through time and materials, basically the amount of hours spend by developers. For each project, there could be one or several contracts, although only one contract is valid at at time. A project could start off as soon as the contract is signed with an initial duration of six months and certain conditions. After the contract is finished a new one could be signed so that the project could go on for another bunch of months and perhaps different terms and conditions - different rates perhaps. 

During the length of a contract the number of developers working on a project don't usually change although they could. The amount of hours spent may certainly fluctuate as some people could get sick or go on vacation. The rates per hour and seniority level don't change. The seniority level of a developer doesn't change during the duration of the contract. 

At the end of each worked month, the software is used to create an invoice with the total cost of development (hours per person) plus commissions, in case certain comissions apply. 

The goal of the kata is to think of a design that support the calcultation of the monthly invoice. 
