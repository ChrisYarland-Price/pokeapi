# POKEAPI
## Task

We were tasked with testing an online api: <https://pokeapi.co/> and had to plan how to test the api.

As a group, we discussed how our Kanban board should be set out. The board consited of the following columns:

* Prioritise; 1 being high and 3 being low
* Execute
* Review
* Definition of done; has the code been peer reviewed and has it been indented properly, implementing DRY.

We then derived user stories which would assist us in creating our test cases/conditions, which were priortised from 1-3; 1 being the test which tests the most functional aspect of the API. Each member of the group took responsibilty on which user story they wanted to complete.

## Tasks undertaken by each member

#### Chris 
I tested each endpoint in the pokemon resource to return the code 200 when given a valid ID.
I tested each endpoint in the pokemon resource for the return of data, by looking for the keys that were supposed to be returned with each query. 
I tested each endpoint in the pokemon resource for the return of the ID that was queried in order to test if it gets back the entry. 

I tested every endpoint that could take a name as a variable, that it returns HTML code 200 and returns valid data.


####Martha
I tested each endpoint in Encounters, Evolution and Games to return the code 200 when given no ID or a valid ID.
I tested each endpoint in Items to return the ID given and a name as a string.

#### Liam
I tested each endpoint for both the berry and contest resources as well as their sub-resources. The tests I wrote test the HTTP response code for the resource lists and first of each resource. Also for the individual instances of the resource I wrote tests to check that the API only returns one thing and that it is the correct thing.  
I got the resource lists for both and the first of each before all the tests start. By using the
```before(:all) do  end```
syntax. This saves making requests in each test and makes the tests easier to read.

#### Luke
Luke created the get resource method which allowed tests on each spec checking that the request would work with only the resource name and doesn't need an ID.
Checked locations and utility return valid data.

#### James
made tests for checking that list requests return code 200 and made tests to check each attribute also returns 200; okay. checked all end points to contain valid id data.

#### Abass

* I tested each endpoint in the location/utility resources. Ensuring that its in JSON format and that it returns the 200 code when given a valid ID.

* I tested that given an id for the evolution resources it returns the correct data e.g. a name returns the correct name in a string etc. Getting a key from a nested hash, or a hash within an array.


## Future work
* If we had more time, more specific and robust tests would be created e.g. can we edit or delete entries from the database.
* Create edge cases e.g. does it take an integer when it should take a string etc.
* Making sure the API gives the correct error codes for the relevant requests.
* Use spec_helper.rb
