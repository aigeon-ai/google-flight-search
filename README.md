# Aigeon AI Google Flight Search

## Project Description

Aigeon AI Google Flight Search is a Python-based server application designed to facilitate flight search queries using Google's flight search capabilities. This project leverages the SerpAPI to interact with Google Flights, providing users with a comprehensive tool to search for flights based on various parameters such as departure and arrival locations, travel dates, flight types, and more.

## Features Overview

- **Flight Search Functionality**: Enables users to search for flights using a wide range of parameters.
- **Flexible Query Parameters**: Supports multiple options for specifying departure and arrival locations, including airport codes and location identifiers.
- **Customizable Search Options**: Allows users to define travel preferences such as travel class, number of passengers, and maximum price.
- **Advanced Filtering**: Offers filtering options based on flight duration, number of stops, and departure/arrival times.
- **Multi-City Flight Support**: Facilitates complex itineraries with multiple city stops.

## Main Features and Functionality

1. **Search Flights**: The core functionality of the application is to perform flight searches using the `search_flight` function. This function is highly customizable, allowing users to tailor their search queries to meet specific travel needs.

2. **Parameter Customization**: Users can specify a variety of parameters to refine their search results:
   - **Departure and Arrival Locations**: Accepts both airport codes and location identifiers.
   - **Travel Dates**: Users can set outbound and return dates for round trips.
   - **Flight Type**: Options include round trip, one-way, and multi-city flights.
   - **Travel Class**: Choose from economy, premium economy, business, or first class.
   - **Passenger Details**: Specify the number of adults, children, and infants.
   - **Price and Duration Constraints**: Set maximum price limits and flight duration preferences.

3. **Advanced Search Options**: The application supports additional search parameters such as:
   - **Sort Order**: Sort results by top flights, price, departure time, arrival time, duration, or emissions.
   - **Stop Preferences**: Filter flights based on the number of stops.
   - **Time Windows**: Define specific time ranges for departures and returns.
   - **Layover and Duration Limits**: Set constraints on layover duration and total flight time.

4. **Multi-City Itineraries**: The application can handle complex travel plans involving multiple destinations, allowing users to specify detailed itineraries with multiple legs.

## Main Function Description

### `search_flight`

The `search_flight` function is the primary tool provided by the application for querying flight information. It is designed to accept a comprehensive set of parameters that allow users to customize their flight search. Key parameters include:

- **departure_id**: Specifies the departure location using airport codes or location identifiers.
- **arrival_id**: Specifies the arrival location using airport codes or location identifiers.
- **gl** and **hl**: Define the country and language settings for the search.
- **type**: Determines the type of flight (round trip, one-way, or multi-city).
- **outbound_date** and **return_date**: Set the travel dates for outbound and return flights.
- **travel_class**: Select the desired travel class.
- **multi_city_json**: Provides detailed itinerary information for multi-city flights.
- **adults**, **children**, **infants_in_seat**, **infants_on_lap**: Specify the number of passengers.
- **sort_by**: Choose the sorting order for the search results.
- **stops**: Filter results based on the number of stops.
- **bags**: Specify the number of carry-on bags.
- **max_price**: Set a maximum price for the flight tickets.
- **outbound_times** and **return_times**: Define time ranges for departures and returns.
- **layover_duration** and **max_duration**: Set constraints on layover times and total flight duration.
- **departure_token** and **booking_token**: Used for selecting specific flights and obtaining booking options.

This function is designed to be flexible and powerful, providing users with the ability to perform detailed and precise flight searches tailored to their specific travel needs.