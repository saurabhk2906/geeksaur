 * In this project SpringFrame work is Used.
 
* Language Used is JAVA

* Layer used to connect UI with data base are 
  * controller layer,
  * Service layer and
  * Repo layer.

* Data Structure Used is based on OOPS concept
* This Project give us information about user,its address,its userid and its phone number.

```
package com.geekster.SampleApplication.Controller;

import org.json.JSONObject;
import org.springframework.web.bind.annotation.*;

@RestController
public class CatController {
    @GetMapping(value="/cat")
    public String getController(@RequestBody String requestData){
        return "get mapping"+requestData;
    }
    @PostMapping(value="/cat")
    public String savecat(@RequestBody String requestData){
        return "post mapping" + requestData;
    }

}
```