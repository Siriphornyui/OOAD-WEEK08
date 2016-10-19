#OOAD HOMEWORK08
##USE CASE DIAGRAM

USE CASE1

CODE

```
:Student:
:Teacher:
:Member:
:Librarian:
:Student: --> :Member:
:Teacher: --> :Member:
:Member: --(Borrow book)
:Member: --(Return book)
:Librarian: --(Checking member)
:Librarian: --(Return book)
:Librarian: --(Borrow book)
:Librarian: --(Checking period borrowed)
:Librarian: --(Calculation fine) 
(Calculation fine) ..>(Checking period borrowed)
(Borrow book)..>(Checking member)
(Return book)..>(Checking period borrowed)
```
DIAGRAM

<img src = "https://github.com/Siriphornyui/OOAD-WEEK08/blob/master/libary.png">


USE CASE2

CODE

```
:Customer:
:Seller:
:Customer:-down-(Buy Product)
:Customer:-down-(Proof of purchase)
(Buy Product)..(dilapidated product within 7 days)
(dilapidated product within 7 days)--(Change within 7 days)
(Proof of purchase)--(Change within 7 days)
:Seller:-up-(Sell Product)
:Seller:.up.(Change within 7 days)
:Seller:.up.(Check Product 7-14day)
(Check Product 7-14day)-up-(Return Product)
:Customer: -down-(Return Product)
```
DIAGRAM

<img src = "https://github.com/Siriphornyui/OOAD-WEEK08/blob/master/%E0%B8%AA%E0%B8%B4%E0%B8%99%E0%B8%84%E0%B9%89%E0%B8%B2.png ">

USE CASE3

CODE

```
:Patient:
:Doctor:
:Nurse:
:Clerk:

:Patient:-down-(Queue)
:Patient:.down.(Canceled)
:Patient:--(Palliate)
:Patient:-down-(Pharmary)
:Patient:-down-(Pay)

:Nurse:-up-(Queue)
:Nurse:-up-(Canceled)
:Nurse:-up-(Pharmary)

:Doctor:--(Palliate)
:Clerk:-up-(Pay)
```
DIAGRAM

<img src = "https://github.com/Siriphornyui/OOAD-WEEK08/blob/master/doctor.png ">

USE CASE4

CODE

```
:Customer:
:Officer:

:Customer:-right-(Checking)
:Customer:-down-(Reservation)
:Customer:--(Payment)
(Reservation).down.(Login)
(Login)-left-(Payment)
(Payment)..(Cash)
(Payment)..(Transfer)


:Officer:-up-(Payment)
:Officer:-up-(Login)
:Officer:-right-(Reservation management)
```
DIAGRAM

<img src = "https://github.com/Siriphornyui/OOAD-WEEK08/blob/master/%E0%B9%82%E0%B8%A3%E0%B8%87%E0%B9%81%E0%B8%A3%E0%B8%A1.png ">

USE CASE5

CODE

```
:Customer:
:Online store:

:Customer:--(Search store)
:Customer:-down-(Select Product)
:Customer:--(Add Line Store)
:Customer:--(Payment)

(Payment)..(Cash)
(Payment)..(Transfer)

:Online store:-up-(Payment)
:Online store:-up-(Delive)
(Delive)..(Post Office)
(Delive)..(Car,Van)
(Delive)..(Meet)
```
DIAGRAM

<img src = " https://github.com/Siriphornyui/OOAD-WEEK08/blob/master/onlinrstore.png">
