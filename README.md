# База даних аеропортy
**Лабораторна робота 1**

**студент групи КП-83 Зрайко Владислав**

## Сутності:
* Flight: (політ)
    * FlightID (Primary Key)
    * AirportID (Foreign Key)
    * PlaneID (Foreign Key)
    * DepartureTime
* Plane (літак)
    * PlaneID (Primary Key)
    * PlaneType
    * Capacity
* Passenger (пасажир)
    * PassengerID (Primary Key)
    * FirstName
    * LastName
    * BirthDate
* Airport (аеропорт)
    * AirportID (Primary Key)
    * AirportName
    * Country
* Reservation (бронювання)
    * ReservationID (Primary Key)
    * FlightID (Foreign Key)
    * PassengerID (Foreign Key)
    
## Зв'язки:
* Many To Many: між Flight та Passenger за допомогою таблиці Reservations
* One to Many: між Plane та Flight, Airport та Flight
   
## ER Diagram
![1](https://github.com/theeverlong/AirportDatabase/blob/main/erd.png)

## DB Structure
![1](https://github.com/theeverlong/AirportDatabase/blob/main/db.png)

## PG4 Screenshots
![1](https://user-images.githubusercontent.com/47531496/94867753-7f042080-044a-11eb-8525-6672d14e6205.png)
![image](https://user-images.githubusercontent.com/47531496/94867790-90e5c380-044a-11eb-9d0f-e8a2b3be8530.png)
![image](https://user-images.githubusercontent.com/47531496/94867818-a0650c80-044a-11eb-9260-993be1807f04.png)
