###### HTTP/1.1 Vs HTTP/2
- HTTP is an appication layer *stateless* protocol designed for communication between *web brower* and *web server*.
- HTTP/1.1 is first standardized version of HTTP, published in 1997. After 15 years, Google published SPDY protocol which later went on to become HTTP/2.0 in 2015.
- The large data that is transmitted over web nowadays created overhead for HTTP/1.1 protocol which was not designed for this purpose. So it was not optimizing data
  for efficient tranmission. HTTP/2.0 solved this problem using below methods:
  - It was designed as binary protocol instead of text protocol(HTTP/1.1) so it can't be read and created manually. It allowed for improved optimization techniques.
  - It is multiplexed protocol which means parallel requests can be made on same connection. Two or more requests can't be made at same time in HTTP/1.1.
  - It compressed headers. In HTTP/1.1, multiples requests and responses contained same metadata which is reduntant.
  - It allows server to store data in client cache using server push technique which allowed browser to display data without requesting again from server.
  
###### Objects and their internal representation in JS
