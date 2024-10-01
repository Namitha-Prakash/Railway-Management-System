# Railway Management System

This is a **Railway Management System** built using **Python** that allows users to book train tickets, choose ticket class, coach, select extra food, and manage ticket cancellations. It also integrates with an **SQL database** to store all booking details and user information.

## Table of Contents

- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Database](#database)
- [Technology Stack](#technology-stack)
- [Contributing](#contributing)
- [License](#license)

## Features

- **Ticket Booking**: Allows users to book tickets for trains across major metropolitan cities in India.
- **Class and Coach Selection**: Users can choose the class (e.g., Economy, Sleeper, AC) and coach.
- **Food Selection**: Option to include extra food services during the journey.
- **Ticket Cancellation**: Users can cancel their tickets with specific cancellation policies.
- **Email Confirmation**: Once tickets are booked, a confirmation email is sent to the user.
- **SQL Database Integration**: Stores all user and booking information securely.

## Installation

1. Clone this repository:
    ```bash
    git clone https://github.com/yourusername/railway-management-system.git
    cd railway-management-system
    ```

2. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

3. Set up the SQL database:
    - Import the provided `.sql` file into your SQL database.
    - Update the connection settings in `config.py` with your database credentials.

4. Run the application:
    ```bash
    python railway_management_system.py
    ```

## Usage

1. **Booking a Ticket**:
    - Start the program and follow the prompts to enter details such as destination, date, class, coach, and food options.
    - Once confirmed, your ticket will be booked and a confirmation email will be sent.

2. **Cancelling a Ticket**:
    - Provide your booking ID and follow the cancellation process. Cancellation policies will be applied based on the time of cancellation.

3. **Viewing Bookings**:
    - Retrieve your bookings and see all the details (class, food, coach, etc.) stored in the SQL database.

## Database

The system uses an **SQL database** to store user details and booking information. Below is a summary of the key tables used:

- **Users**: Stores user information such as name, email, and contact details.
- **Bookings**: Contains booking details like train, class, date, and food preferences.
- **Cancellations**: Logs ticket cancellations and applicable refunds.

Ensure that the SQL server is running, and the connection details in `config.py` are correct for smooth database operations.

## Technology Stack

- **Language**: Python
- **Database**: SQL
- **Libraries**: SQLite/MySQL, smtplib (for sending email confirmations)

## Contributing

Contributions are welcome! Please fork this repository and submit a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
