**Cankarjev dom API**
----
  <_Returns the list of events for the requested month._>

* **URL**

  <_https://www.cd-cc.si/koledar/mesec/$month/all_>

* **Method:**
  
  <_GET_>

  `GET` | `POST` | `DELETE` | `PUT`
  
*  **URL Params**

   <_$month = requested month_> 
 
* **Success Response:**
  
  <_What should the status code be on success and is there any returned data? This is useful when people need to to know what their callbacks should expect!_>

  * **Code:** 200 <br />
    **Content:**
    
| Field   |      Type      |  Description |
|----------|:-------------:|------:|
| title |  string | The title of the event. |
| col 2 is |    centered   |   $12 |
| col 3 is | right-aligned |    $1 |

* **Sample Call:**

  <_Just a sample call to your endpoint in a runnable format ($.ajax call or a curl request) - this makes life easier and more predictable._> 

* **Notes:**

  <_This is where all uncertainties, commentary, discussion etc. can go. I recommend timestamping and identifying oneself when leaving comments here._> 
