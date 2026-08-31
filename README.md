# Movie Ticket Booking Management

A Pega Platform application developed for the **Pega National Internship Program (NIP) 2026** to manage the end-to-end movie ticket booking process for CineWave Entertainment.

## Overview

The application replaces manual movie ticket booking through emails and offline systems with a case-based Pega workflow. It allows customers to submit booking requests, enables booking agents to check seat availability, and automates confirmation, seat allocation, ticket generation, and customer notifications.

## Features

- Customer movie ticket booking request
- Movie Name, Show Date, Show Time, Theatre, Show Type, and Number of Tickets
- Movie and Show reusable data objects
- Seat availability checking
- Available Seats Count validation
- Automatic Total Cost calculation
- Customer booking confirmation or cancellation
- Premium and Standard show-based routing
- Seat allocation and Seat Numbers
- Automatic Ticket ID generation
- Booking Confirmation Status
- Booking confirmation email
- SLA management with 1-day goal and 2-day deadline

## Technology

- Pega Platform
- Pega App Studio
- Pega Dev Studio

## Case Type

**Movie Ticket Request**

## Case Lifecycle

### 1. Booking Request
Customer submits:
- Movie Name
- Show Date
- Show Time
- Number of Tickets
- Show Type
- Theatre

### 2. Availability
Booking Agent:
- Checks seat availability
- Enters Available Seats Count
- Enters Ticket Price
- System calculates Total Cost

### 3. Customer Confirmation
Customer reviews the booking summary and can:
- Confirm Booking
- Cancel Booking

### 4. Booking Execution
Confirmed bookings are routed based on Show Type:
- Premium → PremiumShowQueue
- Standard → StandardShowQueue

The system then allocates seats and generates a Ticket ID.

### 5. Resolution
Successful bookings are resolved as **Completed** and a confirmation email is sent to the customer.

## Personas

### Customer
- Submit booking requests
- Review booking summary
- Confirm or cancel bookings
- Receive booking confirmation

### Booking Agent
- Review booking requests
- Check seat availability
- Enter ticket price
- Process bookings
- Allocate seats

## Data Objects

### Movie
- Movie Name
- Genre
- Language
- Duration
- Rating

### Show
- Movie
- Show Date
- Show Time
- Show Type
- Theatre
- Seat Capacity
- Available Seats
- Ticket Price

## SLA

- Goal: **1 day**
- Deadline: **2 days**
- Goal missed: Approaching deadline flag
- Deadline missed: Increased urgency/priority

## Email Notification

Successful bookings generate a confirmation email containing:

- Case ID
- Movie Name
- Show Date
- Show Time
- Number of Tickets
- Seat Numbers
- Total Cost
- Ticket ID
- Booking Confirmation Status

## Developer

**Kowshika Dorraju**

## College

**Vel Tech Rangarajan Dr. Sagunthala R&D Institute of Science and Technology, Chennai**

## Course

**B.Tech – Computer Science and Engineering**

## Internship

**Pega National Internship Program (NIP) 2026**
