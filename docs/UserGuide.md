# User Guide

* [1. Introduction](#introduction)
* [2. Quick Start](#quick-start)
* [3. Features](#features)
    + [3.1. Add:](#add) `add`
    + [3.2. Delete:](#delete) `delete`
    + [3.3. List:](#list) `list`
* [4. Command Summary](#summary)

<a name="introduction"></a>

## Introduction

Restaurant Daily Report is a CLI app that generates a whitepaper, 
summarizing the internals of a restaurant. It’s aim is to provide 
restaurant owners a quick overview of how their restaurant is performing 
daily so that restaurant owners can better manage their business operations.

As such, the daily report will include these categories:
* Menu: Information on all menu items
* Reservation: Information on number of reservations a day
* Stock: Information on all food items/quantities/prices

<a name="quick-start"></a>

## Quick Start

1. Ensure that you have Java 11 or above installed.
1. Down the latest version of `Restaurant Report` from [here](https://github.com/AY1920S2-CS2113-T14-4/tp).

<a name="features"></a>

## Features 

Add menu items, ingredients and reservations.

<a name="add"></a>

### Add
Add menu items, ingredients, and reservations.

#### Add menu item: add dish
* Format: `add dish; n/NAME; [i/INGREDIENT1, INGREDIENT2, ...];`
* Example: `add dish; n/bacon pizza; i/cheese, bacon;`
#### Add ingredient into stock: add stock
* Format: `add stock; i/INGREDIENT1; q/QUANTITY; p/PRICE;`
* Example: `add stock; i/tomato; q/10; p/$0.50;`
#### Add reservation into list: add reservation 
* Format: `add reservation; p/CONTACT_PERSON_NAME; d/DATE; n/NUMBER_OF_GUESTS; c/CONTACT; [m/COMMENTS];`
* Example: `add reservation; r/12;`
*The `DATE` must be in **yyyy-mm-dd HH:mm** format. The `NUMBER_OF_GUESTS` must be an integer.*

<a name="delete"></a>

### Delete
Delete menu items, ingredients and reservations.

#### Delete menu item: delete dish
* Format: `delete dish; n/NAME;`
* Example: `delete dish; n/bacon pizza;`
#### Delete stock of ingredient: delete stock
* Format: `delete stock; i/[INGREDIENT]; q/[QUANTITY];` or
* Format: `delete stock; i/[INGREDIENT];`
* Example: `delete stock; i/tomato; q/1;`
#### Mark reservation as invalid: delete reservation
* Format: `delete reservation; r/NUMBER_OF_RESERVATION;`
* Example: `delete reservation; r/12;`

<a name="list"></a>

### List
List items in the menu, ingredients and reservations.

* List menu : `list menu`
* List ingredients : `list ingredient`
* List reservation : `list reservation`

<a name="summary"></a>

## Command Summary

* Format: `add dish; n/NAME; [i/INGREDIENT1, INGREDIENT2, ...];`
* Format: `add stock; i/INGREDIENT1; q/QUANTITY; p/PRICE;`
* Format: `add reservation; r/NUMBER_OF_RESERVATIONS;`
* Format: `delete dish; n/NAME;`
* Format: `delete stock; i/[INGREDIENT]; q/[QUANTITY];`
* Format: `delete stock; i/[INGREDIENT];`
* Format: `delete reservation; r/NUMBER_OF_RESERVATIONS;`
