# Hotel Management System

## Overview

The **Hotel Management System** is a comprehensive Odoo module designed to streamline hotel operations, focusing on guest registration, room management, and billing. Developed for hotels and similar establishments, this system centralizes guest data, room assignments, and financial transactions, ensuring efficient workflows and improved guest experiences. The project exists to provide a robust, extensible, and user-friendly solution for managing hotel operations within the Odoo ecosystem.

## Key Features

- **Guest Registration:** Manage guest check-in, check-out, and reservation details.
- **Room Management:** Organize rooms by type, track availability, and assign guests.
- **Room Types & Charges:** Define room types, daily charges, and manage pricing structures.
- **Guest Master List:** Maintain detailed guest profiles, including contact information and photos.
- **Hotel Charges:** Configure and manage various hotel charges and billing items.
- **Document Management:** (Planned) Support for storing and managing hotel-related documents.
- **Role-Based Access:** Secure access to features based on user roles (leveraging Odoo security).

## Tech Stack

- **Odoo** (ERP Framework)
- **Python 3** (Odoo module development)
- **XML** (Views, menus, and security definitions)
- **PostgreSQL** (Odoo backend database)

## Prerequisites & Installation

### Prerequisites
- Odoo 15 or later (Community or Enterprise)
- Python 3.7+
- PostgreSQL database
- Git (for cloning the repository)

### Installation Steps

1. **Clone the Repository:**
   ```sh
   git clone https://github.com/GreeceA/hotel.git
   ```
2. **Copy to Odoo Addons Directory:**
   Place the `hotel` folder inside your Odoo custom addons directory.

3. **Update Odoo Configuration:**
   Add the custom addons path to your `odoo.conf` file:
   ```ini
   addons_path = /path/to/odoo/addons,/path/to/your/custom/addons
   ```

4. **Install Required Python Packages:**
   Ensure all dependencies for Odoo are installed (see Odoo documentation).

5. **Restart Odoo Server:**
   ```sh
   ./odoo-bin -c /path/to/odoo.conf
   ```

6. **Activate Developer Mode:**
   In Odoo, go to Settings > Activate the developer mode.

7. **Install the Module:**
   - Go to Apps, search for "Hotel Management System" or `hotel`.
   - Click **Install**.

## Usage Instructions

### Basic Workflow
1. **Define Room Types & Charges:**
   - Go to Hotel > Room Types to create room categories and set daily charges.
2. **Add Rooms:**
   - Go to Hotel > Rooms to add and configure individual rooms.
3. **Register Guests:**
   - Go to Hotel > Guests to add guest profiles.
4. **Create Guest Registrations:**
   - Go to Hotel > Guest Registration to manage reservations, check-ins, and check-outs.
5. **Manage Charges:**
   - Go to Hotel > Charges to define billable items.

### Example: Registering a New Guest
1. Navigate to **Guests** and click **Create**.
2. Fill in guest details (name, contact, photo, etc.).
3. Save the record.
4. Go to **Guest Registration** and create a new registration, selecting the guest and room.
5. Set check-in/check-out dates and confirm the reservation.

## Contributing

Contributions are welcome! To contribute:
1. Fork the repository.
2. Create a new branch for your feature or bugfix.
3. Commit your changes with clear messages.
4. Push to your fork and submit a pull request.

Please follow Odoo module development best practices and ensure your code is well-documented.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
