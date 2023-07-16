# lab-11-Async-Inn

**Project Name:** Async Inn Hotel Asset Management System
**Author:** Abdelrahman shaheen
**Date:** 7/16/2023
## Description
The Async Inn Hotel Asset Management System is a web-based API designed to help Async Inn, a local hotel chain, better manage their hotel assets across multiple locations. This project aims to provide a RESTful API server that allows the management of rooms, amenities, and new hotel locations. The system leverages a relational database to store and maintain the integrity of the data.
## ERD Diagram
![Async-Inn-ERD]()
Explanation of the Tables:
1. **Location**:
   - Represents each hotel location with its unique identifier, name, city, state, address, and phone number.
   - Attributes: location_id (PK), name, city, state, address, phone_number
2. **Room**:
   - Represents individual rooms in each location. Each room has a unique identifier, a nickname for easy identification, a price, and a flag indicating if it is 
    pet-friendly.
   - Attributes: room_id (PK), location_id (FK), nickname, price, pet_friendly
3. **Amenity**:
   - Represents the various amenities that rooms can have, such as air conditioning, coffee maker, etc.
   - Attributes: amenity_id (PK), name
4. **RoomAmenity**:
   - Acts as a pure join table to establish a many-to-many relationship between rooms and amenities.
   - Attributes: room_id (PK, FK), amenity_id (PK, FK)


