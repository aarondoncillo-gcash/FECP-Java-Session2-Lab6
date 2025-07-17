# Name: Ronan Aaron Doncillo
# Lab 6: Define Your REST API Endpoints

| **Resources** | **HTTP verb** | **Resource URL**                                                         | **Use Case Eepresentation**                |
|:-------------:|:-------------:|--------------------------------------------------------------------------|--------------------------------------------|
| Tickets       | POST          | `/tickets`                                                               | Creating a ticket                          |
| Tickets       | GET           | `/tickets/{ticket_num}`                                                  | Getting a ticket with id                   |
| Tickets       | POST          | `/visitors/{visitor_id}/tickets`                                         | Visitor buying a ticket                    |
| Tickets       | GET           | `/visitors/{visitor_id}/tickets`                                         | Get all visitor's tickets                  |
| Tickets       | GET           | `/visitors/{visitor_id}/tickets/{ticket_num}`                            | validate visitor's ticket                  |
| Tickets       | DELETE        | `/tickets/{ticket_num}`                                                  | Delete ticket (void ticket)                |
|               |               |                                                                          |                                            |
| Visitors      | GET           | `/zoos/1/visitors/{visitor_id}`                                          | get visitor options                        |
| Visitors      | POST          | `/visitors`                                                              | Registering(Creating) a visitor            |
| Visitors      | GET           | `/visitors/{visitor_id}`                                                 | Get visitor info                           |
| Visitors      | DELETE        | `/visitors/{visitor_id}`                                                 | Delete visitor (Visitor leave the zoo)     |
|               |               |                                                                          |                                            |
| Enclosures    | GET           | `/zoos/{zoo_id}/enclosures/{enclosure_id}`                               | get species enclosure                      |
|               |               |                                                                          |                                            |
| Animals       | GET           | `/zoos/{zoo_id}/enclosures/animals/{species}/{type}`                     | get all animals from a specific type       |
| Animals       | GET           | `/zoos/{zoo_id}/enclosures/animals/{species}/{type}/{animal_id}`         | get a specific animal                      |
| Animals       | PATCH         | `/zoos/{zoo_id}/enclosures/animals/{species}/{type}/{animal_id}`         | update animal's location                   |
| Animals       | POST          | `/zoos/{zoo_id}/visitors/{visitor_id}/animals/{animal_id}`               | feed a specific animal by a visitor        |
|               |               |                                                                          |                                            |
| Shops         | GET           | `/zoos/{zoo_id}/shops/{shop_id}`                                         | get all items in a shop                    |
| Shops         | POST          | `/zoos/{zoo_id}/visitors/{visitor_id}/shops/{shop_id}`                   | make purchase in a shop                    |
| Shops         | PATCH         | `/zoos/{zoo_id}/shops/{shop_id}/items/{item_id}`                         | update item's price                        |
| Shops         | GET           | `/zoos/{zoo_id}/shops/{shop_id}/items/{item_id}`                         | get specific item from a shop              |
| Shops         | POST          | `/zoos/{zoo_id}/shops/{shop_id}/items`                                   | insert new item                            |
|               |               |                                                                          |                                            |
| Hospitals     | POST          | `/zoos/{zoo_id}/visitors/{visitor_id}/hospitals/{hospital_id}`           | attend the science lecture in the hospital |
| Hospitals     | GET           | `/zoos/{zoo_id}/hospitals/{hospital_id}/veterinarians/{veterinarian_id}` | get available veterinarian                 |
