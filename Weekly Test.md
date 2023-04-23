 * In this project SpringFrame work is Used.
 
* Language Used is JAVA

* Layer used to connect UI with data base are 
  * controller layer,
  * Service layer and
  * Repo layer.

* Data Structure Used is based on OOPS concept
* This Project give us information about restaurant name, restaurant address, number, specialty, total staffs.

Below is Code

```
package com.geekster.restaurant.Controller;

import org.springframework.web.bind.annotation.*;

@RestController
public class CatController {
    @GetMapping(value="/cat")
    public String getRestaurant(@RequestBody String requestData){
        return "This is get Mapping"+requestData;
    }
    @PostMapping(value="/cat")
    public String saveRestaurant(@RequestBody String requestData){
        return "This is post Mapping"+requestData;
    }

}

```