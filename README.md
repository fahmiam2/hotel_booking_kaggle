# Hotel Booking Prediction

# Introduction
## Context
Have you ever wondered when the best time of year to book a hotel room is? Or the optimal length of stay in order to get the best daily rate? What if you wanted to predict whether or not a hotel was likely to receive a disproportionately high number of special requests?

This hotel booking dataset can help you explore those questions!

## Content
This data set contains booking information for a city hotel and a resort hotel, and includes information such as when the booking was made, length of stay, the number of adults, children, and/or babies, and the number of available parking spaces, among other things.

All personally identifying information has been removed from the data.

## Acknowledgements
The data is originally from the article [Hotel Booking Demand Datasets]("https://www.sciencedirect.com/science/article/pii/S2352340918315191"), written by Nuno Antonio, Ana Almeida, and Luis Nunes for Data in Brief, Volume 22, February 2019.

The data was downloaded and cleaned by Thomas Mock and Antoine Bichat for #TidyTuesday during the week of February 11th, 2020.

## Column Description

This data set contains a single file which compares various booking information between two hotels: a city hotel and a resort hotel. This dataset has 32 columns with descriptions as following:

- __hotel__ : Hotel (H1 = Resort Hotel or H2 = City Hotel).
- __is_canceled__ : Value indicating if the booking was canceled (1) or not (0).
- __lead_time__ : Number of days that elapsed between the entering date of the booking into the PMS and the arrival date.
- __arrival_date_year__ : Year of arrival date.
- __arrival_date_month__ : Month of arrival date.
- __arrival_date_week__ : Week number of year for arrival date.
- __arrival_date_day__ : Day of arrival date.
- __stays_in_week_nights__ : Number of week nights (Monday to Friday) the guest stayed or booked to stay at the hotel.
- __adults__ : Number of adults.
- __children__ : Number of children.
- __babies__ : Number of babies.
- __meal__ : Type of meal booked. Categories are presented in standard hospitality meal packages: 
        1. Undefined/SC – no meal package;
        2. BB – Bed & Breakfast;
        3. HB – Half board (breakfast and one other meal – usually dinner);
        4. FB – Full board (breakfast, lunch and dinner)
- __country__ : Country of origin. Categories are represented in the ISO 3155–3:2013 format
- __market_segment__ : Market segment designation. In categories, the term __TA__ means “Travel Agents” and __TO__ means “Tour Operators”.
- __distribution_channel__ : Booking distribution channel. The term __TA__ means “Travel Agents” and __TO__ means “Tour Operators”.
- __is_repeated_guest__ : Value indicating if the booking name was from a repeated guest (1) or not (0).
- __previous_cancellations__ : Number of previous bookings that were cancelled by the customer prior to the current booking.
- __previous_bookings_not_canceled__ : Number of previous bookings not cancelled by the customer prior to the current booking.
- __reserved_room_type__ : Code of room type reserved. Code is presented instead of designation for anonymity reasons.
- __assigned_room_type__ : Code for the type of room assigned to the booking. Sometimes the assigned room type differs from the reserved room type due to hotel operation reasons (e.g. overbooking) or by customer request. Code is presented instead of designation for anonymity reasons	
- __booking_changes__ : Number of changes/amendments made to the booking from the moment the booking was entered on the PMS until the moment of check-in or cancellation.
- __deposit_type__ : Indication on if the customer made a deposit to guarantee the booking. This variable can assume three categories:	BO and TR/Value calculated based on the payments identified for the booking in the transaction (TR) table before the booking׳s arrival or cancellation date.
        1. No Deposit – no deposit was made;
        2. Non Refund – a deposit was made in the value of the total stay cost;
        3. Refundable – a deposit was made with a value under the total cost of stay.
- __agent__ : ID of the travel agency that made the booking.
- __company__ : ID of the company/entity that made the booking or responsible for paying the booking. ID is presented instead of designation for anonymity reasons.
- __days_in_waiting_list__ : Number of days the booking was in the waiting list before it was confirmed to the customer
- __customer_type__ : Type of booking, assuming one of four categories:
        1. Contract - when the booking has an allotment or other type of contract associated to it;
        2. Group – when the booking is associated to a group;
        3. Transient – when the booking isn't part of a group/contract, and isn't associated to other transient booking.
        4. Transient-party – when the booking is transient, but is associated to at least other transient booking
- __adr__ : Average daily rate.
- __required_car_parking_spaces__ : Number of car parking spaces required by the customer.
- __total_of_special_requests__ : Number of special requests made by the customer (e.g. twin bed or high floor).
- __reservation_status__ : Reservation last status, assuming one of three categories:
        1. Canceled – booking was canceled by the customer;
        2. Check-Out – customer has checked in but already departed;
        3. No-Show – customer did not check-in and did inform the hotel of the reason why                    
- __reservation_status_date__ : Date at which the last status was set. This variable can be used in conjunction with the ReservationStatus to understand when was the booking canceled or when did the customer checked-out of the hotel.

## Task
### Task Details
Can we predict the possibility of a booking for a hotel based on cancellation as the target?

# License 

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
