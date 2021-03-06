SOFTWARE GHOSTS

# PHARMAX PRO

```
PHARMACY MANAGEMENT WEB APPLICATION
```

## INTRODUCTION

- **PHARMAX** is a web application designed to manage pharmacies and meet all their
    needs. The application is built on a carefully designed and optimized database and a
    solid system that combines powerful performance with great UI experience.
- **PHARMAX** improves your pharmacy management experience with all the functions it
    comes with, such as viewing data tables, adding or modifying data via simple forms
    that are very user friendly, choosing between multiple themes that gives you the best
    color experience, securing your data and providing different account types with
    different privileges that satisfy managers’ needs. Moreover, this application is being
    developed and improved by time as we try to improve our ideas and get best out of
    users’ feedbacks. We hope you will have a great experience using **PHARMAX** and get
    best out of it.
- This application is created by _Software Ghosts_ ; a team of five 3 rd year Computer
    Engineering students “ _Ahmed Bally, Abdelrahman Abdelhamid, Abdelrahman_
    _Metwaly, Mohamed Adam and Mona Mardy_ ” supervised by Prof. Dr. Amany Sarhan.

### USER TYPES AND PRIVILEGES

```
(Admin) Full Access
- View all data tables.
- Add, update or remove existing data.
```
```
(Pharmacist) Partial Access
- Create invoices.
- View customers, medicines and inventory data
- Manage medicines, inventory and customers data.
```
```
(Sales) Partial Access
- View pharmacies, customers, invoices, inventories and suppliers’ data.
- Manage medicines, customers and suppliers data.
```

## DASHBOARD

(1) Navbar Buttons

- Notifications – alerting medicines status.
- Account Settings – quick access to account, app settings and logout.

(2) Recent Stats Panels

- New Customers – no. of new customers registered within last week.
- New Invoices – no. of new invoices printed within last week.
- Need Restock – no. of medicines running out of stock
- Expire Soon – no. of medicines expiring in 3 months.

(3) Statistics

- Sales Comparison – total sales from each pharmacy branch.
- Branches Sales – total no. of items sold from each pharmacy branch.


## REPORTS

- Sales – advanced sales charts.
- Logs – saving all employees action for further reviews by managers.
    Both reports sections are not available yet.

## TABLES

- Display data stored in the pharmacy database.
- Tables as displayed are summarized in the following structure:

* Inventory table shows products in stock for each different pharmacy branch.

**[Table] - Displayed Columns**
```
[Pharmacies]:	Pharmacy	| Location | Phones	| Admin	| Admin Phone						
[Employees]:	Employee ID	| Pharmacy | First Name	| Last Name | Employee Phone | Address | Type | Salary | Shift | Hire Date | Photo
[Customers]:	Customer ID	| Name	| Address	| Phone	| Score					
[Invoices]:	Invoice ID	| Items | Employee Name	| Customer Name	| Print Date	| Total	| Pharmacy	
[Inventory]:	Product ID	| Name	| Price	Quantity | Expire Date	| Barcode					
[Medicines]:	Medicine ID	| Name	| Description	| Supplier ID	| Supplier Name						
[Suppliers]:	Supplier ID	| Name	| Phone	Address	| Email						
```

### TABLES FEATURES

1. Data tables are displayed according to **user type** (privilege dependent).
2. Clear and not confusing display of data for each table.
3. Dynamic **search** within all columns that works on typing, for each table.
4. Choose number of rows to be displayed per page.
5. All tables support **sorting** by any column.

### MANAGEMENT – INVOICES

- Manage selling process by creating new invoices for customers through
    the **Invoices Panel** – Management > Invoices.
**1. Adding medicines**
    a. Search for medicines by their name or barcode.
    b. Results will show up on typing, must click the medicine name to add.
    c. Only medicines in current user’s pharmacy’s inventory will appear.
**2. Modifying invoice list**
    a. You can modify quantity of each medicine as desired.
    b. Delete button is available to remove a medicine from the invoice.
    c. Total price will be updated on any change.
**3. Registering customer** (optional)
    a. Register a new customer or assign
       existing one to this invoice.
    b. On typing the customer’s phone
       number, the number would show up
       by auto completion if it already exists
       in the database, must click the result
       for rest of the customer’s data to be
       filled automatically.
    c. Click _Confirm & Print_ to print the invoice.

### DATA MANAGEMENT

- **Add** , **Update** or **Delete** data to / from the tables:
    _Pharmacies, Employees, Customers, Inventory, Medicines and Suppliers._
1. **Adding** a new branch to the database requires the new branch’s _address_
    and _phone_ number(s) then **Submit**. _Pharmacy number_ should be ignored.
    **Administrator** employee is assigned to the new branch after creation,
    using _modify an existing branch_ form.


2. To **Modify** an existing branch, select the pharmacy from the list, change
    desired values and _Admin Employee_ then apply changes. You can **remove**
    this branch from the database using _Remove Branch_ button.

**Supplier Management** is very similar in functionality to the previous example.

Rest of management pages _“Employees – Customers – Inventory – Medicines”_
are similar, with two sections on each page, one for **adding** and another one for
**modifying** , but there are few differences:

1. **Modifying** any data record from the previous tables using _modify_ section
    in each one’s page requires _searching_ for the _desired record_ with the
    specified value in _placeholder_ , and then must click on a result that is
    shown by auto completion to select that record.
2. **Adding** a new item to any of these tables is similar, simply fill form with
    the required data then click _Submit Button_.

NOTE that a **Success** message will always show up on cases of successful operation,
for any of the app functions. **Failure** message will show up otherwise.

### MANAGEMENT – ADDING PRODUCTS

- In PHARMAX **medicines** and **products** are not the same.
- Medicines represent the data from which we create products; this solves
    problems like having different units from the same medicine with different
    production and expire dates or different barcodes.
- **To add a medicine product (that can be added to invoices):**
    1. **Add** the medicine to your database using _Add form_ in **Medicines**
       **management** page, as shown in previous example. This requires
       Medicine’s _name_ , _description_ and _Supplier_.
    2. Note that you must specify the supplier, therefore you must make sure
       the medicine’s supplier is added previously using _Supplier management_
       page. If not, you might need to add it first.
    **3. After adding the medicine,** go to
       **Inventory management** page, where you can add new products to selected pharmacy’s inventory
       (or update existing products, of course).
    **4.** You will need to _search_ for the medicine and must click on one
       result from the auto completion, select the _pharmacy_ and enter
       product’s _price_ , _quantity_ , _expire__date_ and _barcode_ , then _submit_.

### MANAGEMENT – DATA FORMATS

- Adding or modifying any data as shown before is a simple process.
    However, you must know the accepted data formats or patterns to have a
    proper accepted input. The following table shows the accepted format for
    each field you would see in any of the forms.

**Field Name**	Accepted Format
**Name**	A string in English alphabet with spaces allowed between words.
**First Name**	A string in English alphabet up to 25 characters.
**Last Name**	A string in English alphabet up to 25 characters.
**Username**	A string starting with (A-Z, a-z) character, followed by same characters, numbers, backslash, underscore or dots. Maximum 20 characters.
**Password**	A string in any characters with minimum length of 5.
**Address**	A string in any characters.
**Salary**	A number in 0 to 9 with minimum length of 3.
**Phone**	A number in 0 to 9 only, with minimum length of 7 and maximum length of 15.
**Description**	A string in any characters.
**Email Address**	A string in proper email address format, e.g. name@site.com


## ORGANIZING

- **Notifications** page displays tables containing the following data:
    **1. Expire Soon** – all medicines expiring in less than 3 months.
    **2. Expired** – all medicines that are already passed expire date.
    **3. Need Restock** – all medicines which quantity are below 10.
- Each section displays info related to its notification.
- All _Table Features_ work on notifications tables as well.

### SCHEDULE

- This feature is not available yet but is expected to be added in next
    versions to help scheduling and managing the pharmacy process and its
    related work.


### APPLICATION SETTINGS

- PHARMAX cares about UI and user experience using the application,
    therefore it supports theming. In App Settings page you can find 4
    different themes to choose from.
- The Popup buttons are added to preview success or error popups.


### ACCOUNT SETTINGS

- There are two sections in _Account Settings_ page
    1. **Current Info** – displays information about the user currently logged-
       in and displays the profile picture.
    2. **Update Info** – contains a form that allows you to update your data,
       password or profile picture. You must enter your current password
       to be able to save any changes.


