# 🚲 Bike Rental Shop (Bash + PostgreSQL)

This project is a **command-line Bike Rental Shop application** built using **Bash scripting and PostgreSQL**.
It was created as part of the **Relational Database Certification** from freeCodeCamp.

The application allows users to **rent bikes, return bikes, and manage customer rental records** through a simple terminal interface.

---

## 📌 Features

* View available bikes
* Rent a bike
* Return a rented bike
* Register new customers automatically
* Store customer and rental information in a PostgreSQL database
* Update bike availability after rental or return

---

## 🛠 Technologies Used

* Bash Scripting
* PostgreSQL
* psql Command Line Interface
* Linux Terminal

---

## 🗄 Database Structure

The project uses three main tables.

### Bikes Table

| Column    | Description                             |
| --------- | --------------------------------------- |
| bike_id   | Unique ID for each bike                 |
| type      | Type of bike (Mountain, Road, etc.)     |
| size      | Bike size                               |
| available | Indicates whether the bike is available |

---

### Customers Table

| Column      | Description           |
| ----------- | --------------------- |
| customer_id | Unique customer ID    |
| name        | Customer name         |
| phone       | Customer phone number |

---

### Rentals Table

| Column        | Description                          |
| ------------- | ------------------------------------ |
| rental_id     | Unique rental ID                     |
| customer_id   | Customer renting the bike            |
| bike_id       | Bike being rented                    |
| date_rented   | Date and time when bike was rented   |
| date_returned | Date and time when bike was returned |

---

## ⚙️ How the Program Works

When the script runs, the user sees the main menu:

```
~~~~~ Bike Rental Shop ~~~~~

How may I help you?

1. Rent a bike
2. Return a bike
3. Exit
```

### Rent a Bike

1. The system shows all available bikes.
2. The user selects a bike.
3. The system asks for the customer's phone number.
4. If the customer is new, their name is requested and stored.
5. A rental record is created and the bike becomes unavailable.

### Return a Bike

1. The system asks for the customer's phone number.
2. It displays the bikes currently rented by the customer.
3. The user selects which bike to return.
4. The return date is recorded.
5. The bike becomes available again.

---

## ▶️ How to Run the Project

Clone the repository:

```
git clone https://github.com/padamdamai/Bike-Rental-Shop-using-postgres.git
```

Move into the project folder:

```
cd Bike-Rental-Shop-using-postgres
```

Run the script:

```
bash bike.sh
```

---

## 📷 Example Output

```
~~~~~ Bike Rental Shop ~~~~~

How may I help you?

1. Rent a bike
2. Return a bike
3. Exit
```

---

## 🎓 Project Source

This project was completed as part of the **Relational Database Certification** from freeCodeCamp.

---

## 📜 License

This project is open source and intended for educational purposes.
