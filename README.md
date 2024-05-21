# Booking System Smart Contract

# Overview

This Solidity smart contract, named `BOOKING_SYSTEM`, facilitates booking services and payment management on the Ethereum blockchain. It provides functionalities for users to manage their budgets for booking services and handles payments for bookings. Below are the key functions provided by this contract:

# Functions

MyBudget
    Description: This function allows users to add funds to their total budget for booking services. It ensures that the payment amount is within specified limits to maintain the integrity of the booking system.
    Parameters:
      `_peso` (uint256): The amount of currency units (assumed to be in Peso) to be added to the user's total budget.
 Constraints
      The payment amount should be greater than 20 Peso.
      The payment amount should not exceed 1000 Peso to prevent overfunding.

bookingpaid
    Description: This function calculates the remaining amount to be paid for kilometers traveled based on the price per kilometer and the amount already paid. It ensures that the user has paid enough for the kilometers traveled.
    Parameters:
   `_perKM` (uint256): The price per kilometer for the booking.
   `_KMpaid` (uint256): The amount paid for kilometers traveled.
Returns
    uint256: The remaining amount to be paid for kilometers traveled.

handleBookingAndPayment
     Description: This function handles the payment process for bookings. It deducts the specified payment amount from the user's total budget, ensuring that the user has sufficient funds to cover the booking expenses.
Parameters:
   `_paymentAmount` (uint256): The amount to be deducted from the user's total budget for the booking.

# License

This smart contract is licensed under the MIT License, allowing users to freely use, modify, and distribute the code. Refer to the SPDX-License-Identifier tag within the contract file for detailed licensing information.

# owner
Raffy Apalla
