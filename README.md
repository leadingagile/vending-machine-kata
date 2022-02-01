# Vending Machine Kata

In this simple kata, your task is to recreate the workings of a vending machine. This vending machine will have a set of products at varying quantities and prices that can be chosen and dispensed.

## Features

### Select a Product

There are three products available in this vending machine. Each product is able to be selected by sending the appropriate code to the machine.

| Item  | Price | Code |
|-------|-------|------|
| Soda  | $1.00 | A01  |
| Chips | $0.65 | A02  |
| Candy | $0.85 | A03  |
| Gum   | $0.40 | A04  |

#### Exact Change

When the respective vending code is entered and the correct amount of money is given, the machine prints "Vending Item Name" where `Item Name` is the name of the item that was selected.

Example output:

```
Vending Soda
```

#### Insufficient Funds

When the respective vending code is entered and not enough money is supplied to the machine, the machine prints "Price: Item Price" where `Item Price` is the actual price of the item selected. The item price should always display two decimal places.

Example output:

```
Price: $0.40
```

#### Returning Change

When the respective vending code is entered and more money than is needed is supplied to the machine, the machine prints "Vending Item Name: Change Item Change" where `Item Name` is the name of the item selected and `Item Change` being the amount of change to be returned. The item's change should display two decimal places.

Example output:

```
Vending Gum: Change $0.60
```

#### Invalid Product

When a vending code is entered that does not exist, the machine prints "Invalid Selection: Item Code" where `Item Code` is the code that was sent to the machine.

Example output:

```
Invalid Selection: A08
```

#### Manage Quantities

The vending machine needs to keep track of how many of each item is in the machine. Whenever an item is selected, it's quantity should be reduced by 1.

#### Out of Stock Item

When a vending code is entered where the quantity of an item is 0, the machine prints: "Sold Out: Item Name" where `Item Name` is the name of the item that is sold out.

Example output:

```
Sold Out: Candy
```
