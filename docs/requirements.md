# Requirements

## User Needs

### User stories
As a food consumer, I want to be able to search for food hygiene ratings of restaurants I desire to eat from so that I can avoid contracting illness arising from food poisoning.

As an owner of a food delivery platform, I want to be able to incorporate food hygiene ratings of the restaurants I offer services to in order to help give food consumers more information regarding restaurants they opt to dine from as well as avoid delivering contaminated food for which I could be held liable. 

As an owner of a restaurant, I want to be able to search for food hygiene ratings displayed on the internet and identify whether or not they are accurate in order to know if food consumers have a proper view of my restaurant.

### Actors
- Food Consumers
- Government Food and Health Agencies
- Food Delivery Platforms
- Restaurant Owners

### Use Cases

| UC1 | SEARCH FOR HYGIENE RATINGS OF PROSPECTIVE RESTAURANTS | 
| -------------------------------------- | ------------------- |
| **Description** | Allows one to look up food hygiene ratings of restaurants within Bristol. |
| **Actors** | Food Consumers |
| **Assumptions** | User knows the specific restaurant they are making an enquiry on. |
| **Steps** | <ul><li>Search for restaurant by name</li><li>View food hygiene ratings and inspection date</li><li>Use information to discern suitability of restaurant for dining requirements</ul> |
| **Variations** | Compare the hygiene ratings of two or more different restaurants using application comparison feature. |
| **Non-functional** | Servers hosting the application should be constantly online. |
| **Issues** | Outdated ratings on the Food Hygiene Ratings Dataset on Open Data Bristol. |

| UC2 | CHECK WHETHER THE HYGIENE RATINGS ARE UP-TO-DATE | 
| -------------------------------------- | ------------------- |
| **Description** | Enables one to check and confirm whether the food hygiene ratings posted on the application are valid. |
| **Actors** | Government Food and Health Agencies, Restaurant Owners |
| **Assumptions** | User has access to records having up-to-date hygiene ratings of their specific restaurant. |
| **Steps** | <ul><li>Search for a restaurant by name. </li><li>View its respective food hygiene rating.</li><li> Compare the rating with the one saved in relevant records.</li></ul> |
| **Variations** | Send a request through the email linked on the website to have a falsely displayed food rating changed. |
| **Non-functional** | Servers hosting the application should be constantly online. |

| UC3 | OBTAIN HYGIENE RATINGS TO DISPLAY IN THEIR APPLICATIONS  | 
| -------------------------------------- | ------------------- |
| **Description** |  Allows one to look up food hygiene ratings of restaurants within Bristol and use that information for display in their respective applications. |
| **Actors** | Food Delivery Platforms |
| **Assumptions** | User knows the specific restaurant they offer delivery services to. |
| **Steps** | <ul><li>Search for restaurants by name.</li><li>View the respective food hygiene ratings.</li><li>Use information gained to display food hygiene ratings in their applications.</li></ul> |
| **Non-functional** | Servers hosting the application should be constantly online. |

![Use-Case Diagram](images/UseCaseDiagram.png)

## Software Requirements Specification
### Functional requirements
#### UC1: SEARCH FOR HYGIENE RATINGS OF PROSPECTIVE RESTAURANTS
- FR1.1: The system shall find restaurants by name from the Safe Food Bristol database.
- FR1.2: The system shall query the database for food hygiene ratings from Open Data Bristol.
- FR1.3: The system should provide a comparison feature between two or more restaurants on food hygiene ratings from Open Data Bristol.

#### UC2: CHECK WHETHER THE HYGIENE RATINGS ARE UP-TO-DATE
- FR2.1: The system shall find restaurants by name from the Safe Food Bristol database.
- FR2.2: The system shall query the database for food hygiene ratings from Open Data Bristol.
- FR1.3: The system should display an email address for inquiries concerning the food hygiene ratings displayed.

#### UC3: OBTAIN HYGIENE RATINGS TO DISPLAY IN THEIR APPLICATIONS
- FR3.1: The system shall find restaurants by name from the Safe Food Bristol database.
- FR3.2: The system shall query the database for food hygiene ratings from Open Data Bristol.

### Non-Functional Requirements
- NFR1.1: The system shall accurately display the food hygiene ratings from Open Data Bristol.
- NFR1.2: The system shall prevent the food hygiene ratings from being altered or tampered with without authorisation.
- NFR1.3: The system should handle unexpected service errors without crashing the entire application.
- NFR1.4: The system should recover automatically or restore normal operation following a failure.
- NFR1.5: The system shall display legible and visually appealing information.
- NFR1.6: The system should respond to user requests within 2 seconds under normal operating conditions.
- NFR1.7: The system shall have a simple and easily navigable interface.
- NFR1.8: The system should be able to easily accommodate changes to the food hygiene ratings displayed wherever necessary.
- NFR1.9: The system shall provide consistent functionality across desktop, tablet and mobile device browsers. 
- NFR1.10: The system should ensure that all implemented functionalities operate in accordance with the defined regulatory obligations, organisational policies and applicable technical standards.


