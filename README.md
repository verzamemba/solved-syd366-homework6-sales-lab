Download Link: https://assignmentchef.com/product/solved-syd366-homework6-sales-lab
<br>
Sale Module

Christy’s customers are individuals in her community, some of whom have have multiple pets.

Christy has developed a list of services by species.  For example, she washes and grooms dogs, washes cats and trims nails, trims nails for guinea pigs and trims nails and files teeth for rabbits. Her prices depend on the size of the animal and the condition of animal.

Christy would like a system that helps her record sales for customers.  Ideally, she would like to be able to retrieve sales for customers, so that she can see what happened in the past.  Also, she would like to see how much money she makes working with different species.

Your task is to create a class diagram and sequence diagrams to support the following user stories and systems usecase specifications.

Use Case: Maintain Customer

User Story

As the owner of this business, I would like to record my customer’s contact information and a list of the pet’s that they own.  Recording pet species, breed, gender and birth year will aid me in preparing for my customer visits.

Acceptance Criteria:

<ol>

 <li>Must be able to record multiple pets for a customer</li>

 <li>Must be able to flag a pet as not serviceable (example: dog bites)</li>

 <li>Must be able to query pets by species.</li>

 <li>Must be able to query sales by customer.</li>

</ol>




Use Case Descriptions

<table>

 <tbody>

  <tr>

   <td width="123">Use Case Name</td>

   <td colspan="3" width="500">Create Customer Information</td>

  </tr>

  <tr>

   <td width="123">Triggering Event</td>

   <td colspan="3" width="500">New customer requests services.</td>

  </tr>

  <tr>

   <td width="123">Brief Description</td>

   <td colspan="3" width="500">Allows the Owner to record a new customer’s information.</td>

  </tr>

  <tr>

   <td width="123">Actors</td>

   <td colspan="3" width="500">Owner</td>

  </tr>

  <tr>

   <td width="123">Related Use Cases</td>

   <td colspan="3" width="500"> </td>

  </tr>

  <tr>

   <td width="123">Preconditions</td>

   <td colspan="3" width="500">Owner has opened the Main Menu.</td>

  </tr>

  <tr>

   <td width="123">Post Conditions</td>

   <td colspan="3" width="500">Customer is saved to the database.  Sales can be created for the customer</td>

  </tr>

  <tr>

   <td width="123">Flow of activities</td>

   <td colspan="2" width="264">Actor</td>

   <td width="236">System</td>

  </tr>

  <tr>

   <td width="123"> </td>

   <td width="52">1.</td>

   <td width="213">Requests to add a new Customer</td>

   <td width="236">Prompts for Customer name, address, telephone  and email address</td>

  </tr>

  <tr>

   <td width="123"> </td>

   <td width="52">2.</td>

   <td width="213">Enters customer name, address, telephone number and email address</td>

   <td width="236">Verifies that name, address, telephone number and email address have been entered.Creates a unique customer identifierDisplays the customer’s identifier, name, address, telephone number and email addressPrompts to add pets</td>

  </tr>

  <tr>

   <td width="123"> </td>

   <td width="52">loop</td>

   <td width="213">Chooses to add new pet</td>

   <td width="236">Displays a list of pet species for selection</td>

  </tr>

  <tr>

   <td width="123"> </td>

   <td width="52">3.</td>

   <td width="213">Selects a pet species</td>

   <td width="236">Prompts for pet name, breed, birth year, and colour.  Displays a list of pet gender for selection.  Displays a list of breeds for selection.</td>

  </tr>

  <tr>

   <td width="123"> </td>

   <td width="52">4.</td>

   <td width="213">Enters pet name, birth year and colour.  Selects a breed, Selects a pet gender.  Selects a breed.</td>

   <td width="236">Pet name must be entered, breed must be selected, birth year and colour must be entered.  Gender must be selected. Data is validCreates a unique pet identifierDisplays the pet’s information including identifier, name, breed, birth year, colour and gender.</td>

  </tr>

  <tr>

   <td width="123"> </td>

   <td width="52">End loop</td>

   <td width="213">Request to save</td>

   <td width="236">Saves the customer and pets</td>

  </tr>

  <tr>

   <td width="123">Exception Conditions</td>

   <td colspan="3" width="500">·         Owner chooses to cancel adding the customer</td>

  </tr>

 </tbody>

</table>




User Story

As the owner of this business, I would like to record my sales so that I can quickly see how much money I’ve made.

Acceptance Criteria:

<ol start="5">

 <li>Must be able to record multiple services for multiple pets belonging to a customer in one sale</li>

 <li>Must be able to query sales by customer.</li>

</ol>

Use Case Descriptions

<table>

 <tbody>

  <tr>

   <td width="124">Use Case Name</td>

   <td colspan="3" width="508">Create Sales</td>

  </tr>

  <tr>

   <td width="124">Triggering Event</td>

   <td colspan="3" width="508">Customer has requested service and the service is complete</td>

  </tr>

  <tr>

   <td width="124">Brief Description</td>

   <td colspan="3" width="508">Allows the Owner to record a new sales</td>

  </tr>

  <tr>

   <td width="124">Actors</td>

   <td colspan="3" width="508">Owner</td>

  </tr>

  <tr>

   <td width="124">Related Use Cases</td>

   <td colspan="3" width="508"> </td>

  </tr>

  <tr>

   <td width="124">Preconditions</td>

   <td colspan="3" width="508">Owner has opened the Main Menu.</td>

  </tr>

  <tr>

   <td width="124">Post Conditions</td>

   <td colspan="3" width="508">Sales is created and can now be queried</td>

  </tr>

  <tr>

   <td width="124">Flow of activities</td>

   <td colspan="2" width="267">Actor</td>

   <td width="241">System</td>

  </tr>

  <tr>

   <td width="124"> </td>

   <td width="50">1.</td>

   <td width="217">Requests to add a new sale</td>

   <td width="241">Displays a list of customers and prompts for selection</td>

  </tr>

  <tr>

   <td width="124"> </td>

   <td width="50">2.</td>

   <td width="217">Selects a customer</td>

   <td width="241">Prompts for service date</td>

  </tr>

  <tr>

   <td width="124"> </td>

   <td width="50">3</td>

   <td width="217">Enters service date</td>

   <td width="241">Verifies that service date has been entered and generates a unique ale number.  Prompts to select pets.</td>

  </tr>

  <tr>

   <td width="124"> </td>

   <td width="50">loop</td>

   <td width="217">Chooses to add a pet</td>

   <td width="241">Displays a list of pets and prompts for selection</td>

  </tr>

  <tr>

   <td width="124"> </td>

   <td width="50">4.</td>

   <td width="217">Selects the pet</td>

   <td width="241">Prompts to select services</td>

  </tr>

  <tr>

   <td width="124"> </td>

   <td width="50">Loop2</td>

   <td width="217">Chooses to add services</td>

   <td width="241">Displays a list of services including service name and price/hour prompting for selection</td>

  </tr>

  <tr>

   <td width="124"> </td>

   <td width="50">5.</td>

   <td width="217">Selects services that apply</td>

   <td width="241">Adds services to the invoice. </td>

  </tr>

  <tr>

   <td width="124"> </td>

   <td width="50">6.</td>

   <td width="217">Updates hours and price</td>

   <td width="241">Calculates the detail amount (hours * price). Calculates taxes and updates sale total.  Displays the sale total, total taxes, sale service details, prompting for changes to  hours and pricePrompts for another petPrompts to save</td>

  </tr>

  <tr>

   <td width="124"> </td>

   <td width="50">End2</td>

   <td width="217">Until all services for a pet have been selected</td>

   <td width="241"> </td>

  </tr>

  <tr>

   <td width="124"> </td>

   <td width="50">End</td>

   <td width="217">Until pets have been selected.</td>

   <td width="241">Displays the sale total, total taxes, invoice service details and prompts to save</td>

  </tr>

  <tr>

   <td width="124"> </td>

   <td width="50">5.</td>

   <td width="217">Chooses to save</td>

   <td width="241">Saves the sale.Return to the main menu</td>

  </tr>

  <tr>

   <td width="124">Exception Conditions</td>

   <td colspan="3" width="508">·         Owner chooses to cancel adding the sale invoice</td>

  </tr>

 </tbody>

</table>




<table>

 <tbody>

  <tr>

   <td width="125">Use Case Name</td>

   <td colspan="3" width="498">Query Sales by Customer</td>

  </tr>

  <tr>

   <td width="125">Triggering Event</td>

   <td colspan="3" width="498">Owner requires a list of sale details by customer</td>

  </tr>

  <tr>

   <td width="125">Brief Description</td>

   <td colspan="3" width="498">Allows the Owner to retrieve sale details for a specific customer for a specified date range</td>

  </tr>

  <tr>

   <td width="125">petActors</td>

   <td colspan="3" width="498">Owner</td>

  </tr>

  <tr>

   <td width="125">Related Use Cases</td>

   <td colspan="3" width="498"> </td>

  </tr>

  <tr>

   <td width="125">Preconditions</td>

   <td colspan="3" width="498">Owner has opened the Main Menu.</td>

  </tr>

  <tr>

   <td width="125">Post Conditions</td>

   <td colspan="3" width="498">sales are retrieved, totaled and displayed</td>

  </tr>

  <tr>

   <td width="125">Flow of activities</td>

   <td colspan="2" width="252">Actor</td>

   <td width="246">System</td>

  </tr>

  <tr>

   <td width="125"> </td>

   <td width="30">5.</td>

   <td width="222">Requests to query sales (by customer, by date) transactions</td>

   <td width="246">Displays a calendar </td>

  </tr>

  <tr>

   <td width="125"> </td>

   <td width="30">6.</td>

   <td width="222">Selects date range </td>

   <td width="246">Verifies that dates are selected.  Displays a list of customers and prompts for selection </td>

  </tr>

  <tr>

   <td width="125"> </td>

   <td width="30">7.</td>

   <td width="222">Selects a customer</td>

   <td width="246">Retrieves sale detail in the specified date range for the specified customer.Calculate and displays totalsPrompts to exit</td>

  </tr>

  <tr>

   <td width="125"> </td>

   <td width="30">8.</td>

   <td width="222">Request to exit</td>

   <td width="246">returns to the main menu</td>

  </tr>

  <tr>

   <td width="125">Exception Conditions</td>

   <td colspan="3" width="498">Owner requests to cancel query</td>

  </tr>

 </tbody>

</table>




Your tasks:

<ol>

 <li>Create a class diagram to support the above case study and Systems Use Case Specifications</li>

 <li>Create an object level sequence diagram, detailing the Create Customer systems use case specification</li>

 <li>Create an object level sequence diagram, detailing the Create Sales use case specification</li>

 <li>Create an object level sequence diagram, detailing the Query Sales (by customers) system use case specification.</li>

</ol>





