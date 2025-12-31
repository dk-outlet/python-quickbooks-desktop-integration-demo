# Python QuickBooks Desktop Integration Demo

This repository provides practical Python examples for integrating with **QuickBooks Desktop** using the QuickBooks SDK (QBFC/COM or qbXML).

It includes working scripts for common operations such as:
- Authentication / connection setup
- Retrieving orders (invoices, sales receipts)
- Querying and checking inventory levels
- Adding new items to QuickBooks

**Note:** QuickBooks Desktop integration requires Windows and a running instance of QuickBooks Desktop Pro or Enterprise with the company file open.

## Prerequisites

- Windows operating system
- QuickBooks Desktop Pro or Enterprise (any recent version) installed and running
- QuickBooks SDK installed (download from Intuit Developer site)
- Python 3.10 or higher
- `pywin32` package (for COM access)

## Quick Start

1. Clone the repository:
   ```bash
   git clone https://github.com/dk-outlet/python-quickbooks-desktop-integration-demo.git
   cd python-quickbooks-desktop-integration-demo
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Configure your QuickBooks connection:
   - Create a `.qwc` (QuickBooks Web Connector) file or use direct COM connection.
   - Example connection scripts are provided in the respective folders.

4. Run a demo (example: authentication/connection test):
   ```bash
   python src/auth_demo.py
   ```

## Repository Structure

- `/src/auth/` – Connection and authentication examples
- `/src/orders/` – Retrieve invoices, sales orders, and sales receipts
- `/src/inventory/` – Query item inventory and stock levels
- `/src/add_item/` – Add new inventory or non-inventory items
- Each folder contains:
  - Main script(s)
  - Small local README with specific run instructions
  - Sample output/examples

## Troubleshooting Tips

- Ensure QuickBooks is running and logged in as Admin in single-user mode for testing.
- Allow the Python script in QuickBooks when prompted ("Yes, always allow access...").
- Common issues: SDK path not found, firewall blocking, or company file not open.

## Contributing

Feel free to open issues or submit pull requests for improvements or additional examples.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

Happy integrating! 🚀
