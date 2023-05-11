# Airline-Business-Process-Analysis


## Project Description
A major airline company has hired us to assist the executive management in analyzing their current business processes and expanding the company by discovering new opportunities. The first deliverable focuses on flight activity and the analysis of frequent flyers, fare basis, upgrades, frequent flyer miles, special fare promotions, overnight stays, and customer status. The analysis also includes the reservation process and customer care interactions.

## Project Requirements
1. State the modeling process for each business process.
2. Construct a logical data model using any diagramming tool.
3. Translate the logical data model to a physical data model in an Excel file.
4. Create tables in Oracle DBMS and populate them with sample data.
5. Construct SQL queries based on the physical model design to answer business questions.
6. Write a report on different types of indexes and partitions used in data warehousing and their usage.

## Project Team
- Abdelaziz Amin
- Ibrahim Elsayed
- Yousra Mohamed

## Project Structure

### Airline Data Warehouse Model
The data warehouse model follows the Kimball approach with a 2-layer architecture, consisting of an executive's data mart, marketing data mart, finance data mart, and customer care data mart. This approach allows for easier understanding of the business processes and supports the specific requirements of each department.

### Executive's Data Mart
- Business Process: Flights Monitoring
- Granularity: One row per flight
- Dimensions: Airport, Plane, Cancellation Reasons, Flight, Date, Time
- Measures: Total Reserved Seats, Flight Duration, Delay Duration, Plane Capacity, Total Revenue, State of Flight

### Marketing Data Mart
- Business Process: Client Reservation Process
- Granularity: One row per client reservation
- Dimensions: Airport, Flight, Fare Base, Booking Channel, Payment Method, Ticket, Date, Time, Class, Tiers, Frequent Flyer, Client, Client Mapping
- Measures: Fare Price, Additional Luggage Fees, Upgrade Fees, Redeemed Miles, Redeemed Dollars, Miles Earned, Qualification Dollars Earned, Total Discount on Price

### Finance Data Mart
- Business Process: Client Reservation
- Granularity: One row per client reservation
- Dimensions: Airport, Flight, Fare Base, Booking Channel, Payment Method, Ticket, Date, Time, Class, Client
- Measures: Channel Commission, Fare Price, Additional Luggage Fees, Upgrade Fees, Airport Fees, Accumulated Taxes, Passenger Facility Cost, Total Actual Paid

### Customer Care Data Mart
- Business Process: Monitor Actions (Complaints, Inquiries, Ratings)
- Granularity: One row per client communication event
- Dimensions: Airport, Flight, Channel of Interaction, Interaction Type, Case State, Issue Ticket, Date, Time, Class, Client


## Files Included

- `logical_data_model.pdf`: PDF file containing the logical data model diagram.
- `physical_data_model.xlsx`: Excel file containing the physical data model with tables, columns, primary indexes, and foreign indexes.
- `sample_data.sql`: SQL script to create tables in Oracle DBMS and populate them with sample data.
- `queries.sql`: SQL queries based on the physical model design to answer business questions.


Please refer to the respective files for detailed information on each aspect of the project.
