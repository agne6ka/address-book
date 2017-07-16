## Address book project using Symfony.

ToDO:

##### Address
* city, street, home number/apartment number
* related with person one to many

##### Email
* address and type (home, business address)
* related with person one to many

##### Groups
* generate entity PersonsGroup: name, info_text
* make relation with Person:
    - in person - privat $group, mappedby=persons , ManyToMany, targetEntity=PersonsGroup
    - in group - privat $persons, mappedby=groups, ManyToMany, targetEntity=Person
    - in database was added 2 additional columns (both will be related)
* for persons in group.persons loop