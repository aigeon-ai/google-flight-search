# Aigeon AI Google Flight Search

Aigeon AI Google Flight Search is a Python-based server application designed to facilitate the search for flights using Google's search capabilities. This application leverages the SERP API to provide detailed flight search results based on user-defined parameters.

## Features Overview

- **Flight Search Functionality**: Allows users to search for flights by specifying various parameters such as departure and arrival locations, travel dates, flight type, travel class, and more.
- **Flexible Search Options**: Supports multiple search criteria including round trips, one-way, and multi-city flights.
- **Customizable Search Parameters**: Users can customize their search by specifying the number of passengers, travel class, price limits, and more.
- **Integration with SERP API**: Utilizes the SERP API for retrieving search results, ensuring accurate and up-to-date flight information.

## Main Features and Functionality

- **Search Flights**: The core functionality is encapsulated in the `search_flight` function, which allows users to search for flights based on a wide range of parameters.
- **Parameter Customization**: Users can specify detailed search parameters including:
  - Departure and arrival airport codes or location identifiers.
  - Outbound and return dates.
  - Flight type (round trip, one-way, multi-city).
  - Travel class (economy, premium economy, business, first).
  - Number of adults, children, and infants.
  - Sorting options for search results (e.g., price, departure time).
  - Maximum price and flight duration constraints.
- **Multi-City Flight Support**: Supports complex itineraries with multiple legs, allowing users to specify detailed flight paths and times.

## API Endpoints or Main Functions Description

### `search_flight`

The `search_flight` function is the primary tool for querying flight information. It accepts a variety of parameters to tailor the search results to the user's needs:

- **departure_id**: Specifies the departure airport code or location identifier.
- **arrival_id**: Specifies the arrival airport code or location identifier.
- **gl**: Country code for the Google search.
- **hl**: Language code for the search.
- **type**: Defines the type of flight (round trip, one-way, multi-city).
- **outbound_date**: Date of departure.
- **return_date**: Date of return (required for round trips).
- **travel_class**: Class of travel (economy, business, etc.).
- **multi_city_json**: JSON string defining multi-city flight details.
- **adults, children, infants_in_seat, infants_on_lap**: Number of passengers.
- **sort_by**: Sorting order of results.
- **stops**: Number of stops allowed.
- **bags**: Number of carry-on bags.
- **max_price**: Maximum ticket price.
- **outbound_times, return_times**: Time ranges for departures and returns.
- **layover_duration**: Duration of layovers.
- **max_duration**: Maximum flight duration.
- **departure_token, booking_token**: Tokens for selecting specific flights or booking options.

## Configuration Parameters Explanation

The application requires configuration through environment variables, specifically:

- **SERP_API_KEY**: This is a crucial environment variable that must be set to authenticate requests to the SERP API. It should be stored securely and loaded using a `.env` file.

This README provides a comprehensive overview of the Aigeon AI Google Flight Search application, detailing its features, functionality, and configuration requirements. The application is designed to offer a robust and flexible solution for flight searches, catering to a wide range of user needs.