# Conference-Ticket-Booking
Welcome to the Conference Ticket Booking System repository! This repository contains the source code and documentation for a system that allows users to book tickets for a conference event. The system is built using Go and provides functionalities for booking tickets, validating user input, and sending confirmation emails.

## Functionalities

The Conference Ticket Booking System provides the following functionalities:

- ### Ticket Booking:
   Users can book tickets for the conference event.
- ### User Input Validation:
   The system validates user input for first name, last name, email address, and number of tickets.
- ### Email Confirmation:
   After booking a ticket, users receive a confirmation email with their ticket details.

## Prerequisites
Make sure you have Go installed on your system.

## Installation
Clone this repository to your local machine or download the source code as a ZIP file.

```
git clone https://github.com/your-username/conference-ticket-booking.git
```

Open a terminal and navigate to the project directory.

```
cd conference-ticket-booking
```

## Usage
Open the main.go file and customize the conference details by modifying the following variables:

```
const conferenceTickets int = 50
var conferenceName = "Go Conference"
var remainingTickets uint = 50
```

Run the following command to execute the Conference Ticket Booking System:
```
go run main.go
```

- The system will display a welcome message and the number of available tickets.

- Follow the prompts to enter your first name, last name, email address, and number of tickets you wish to book.

The system will validate your input and either book the tickets or display an error message if the input is invalid.

- If the input is valid and tickets are available, the system will book the tickets, display a confirmation message, and decrement the number of available tickets.

- In a separate goroutine, a ticket confirmation email will be sent to the provided email address.

- The program will continue running until all tickets are booked or the user decides to exit.

## ## Input and Output

Here's an example of the input and corresponding output based on the provided main.go code:

### Input:

```
Enter your first name:
John
Enter your last name:
Doe
Enter your email address:
johndoe@example.com
Enter number of tickets:
2
```

### Output:

```
Welcome to Go Conference booking application
We have a total of 50 tickets and 50 are still available.
Get your tickets here to attend
Thank you John Doe for booking 2 tickets. You will receive a confirmation email at johndoe@example.com
48 tickets remaining for Go Conference
```

## Why Go is better than other programming languages

- Go is a statically typed language that is easy to read and write.
- Go has a garbage collector that automatically frees up memory.
- Go has built-in concurrency support that makes it easy to write concurrent programs.
- Go has a simple syntax that makes it easy to learn.
- Go has a fast compile time that makes it easy to develop and test code.
- Go has a large standard library that provides many useful packages for developers.
- Go is open source and has a large community of developers who contribute to its development.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.
