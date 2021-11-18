### HTTP/1.1 Vs HTTP/2
- HTTP is an appication layer *stateless* protocol designed for communication between *web brower* and *web server*.
- HTTP/1.1 is first standardized version of HTTP, published in 1997. After 15 years, Google published SPDY protocol which later went on to become HTTP/2.0 in 2015.
- The large data that is transmitted over web nowadays created overhead for HTTP/1.1 protocol which was not designed for this purpose. So it was not optimizing data
  for efficient tranmission. HTTP/2.0 solved this problem using below methods:
  - It was designed as binary protocol instead of text protocol(HTTP/1.1) so it can't be read and created manually. It allowed for improved optimization techniques.
  - It is multiplexed protocol which means parallel requests can be made on same connection. Two or more requests can't be made at same time in HTTP/1.1.
  - It compressed headers. In HTTP/1.1, multiples requests and responses contained same metadata which is reduntant.
  - It allows server to store data in client cache using server push technique which allowed browser to display data without requesting again from server.
  
### Objects and their internal representation in JS
- Javascript is a *prototype* based object oriented language which differs from other *class* based oop implementation in languages like C, Java.
- Object is an important data type of JS which is used to store complex data as key-value pairs. Eg:
  ```js
  let employee = {
        name : "harsha",
        id   : 2021,
        skills : ["java", "webdev"],
        "dept name" : marketing,
        displayInfo: function() {
            console.log(`${employee.name} whose id is ${employee.id} works in department ${employee["dept name"]}.`);
        }
  };
  ```
- As can be seen in above example, both function and data can be encapsulated in an object, same as class properties and methods in java.
- Each property of object can be accessed using `object.key` or `object[key]` syntax. Data is accessed in O(1) time.
- Object can be created in many ways including method as shown above, `Object.create()`, `new` keyword or `constructor`.
- `for..in` can be used to loop over object keys.
