# Calculator API 

A simple calculator  that can process mathematical expressions and return the result, and optionally, the steps taken to calculate the result.

## Features
- Support for binary operators such as addition, subtraction, multiplication, and division.
- Support for unary operators such as negation and positive.
- Support for functions such as sin, cos, tan, sqrt, log, max, min, and pow.
- Support for constants such as pi, tau, and e.
- Support for showing the steps taken to calculate the result.
- Support for caching results to improve performance.

## How to use
1) Run the server.py script. This will start the server and listen for incoming connections on the specified host and port.
2) Run the client.py script. This will connect to the server and send an expression for evaluation.
3) Optionally, a proxy server also present in the repository which can act as a middleman between the client and server and does caching.

### Prerequisites

- Python 3.10 or later.
- The `socket` and `threading` modules.

### Folders and files description
- api.py : contains the data structure and functions for the calculator
- server.py : the server script which listens for incoming connections and processes the requests
- client.py : the client script which sends expression to the server
- proxy.py : the proxy script which acts as middleman between client and server and handle caching

### Caching
- caching is also implemented, so that no need to request the same data again and again
  from the original server.

### Note 
- you can make changes in the the host and port on which the server is listening in the 
  server.py file and in the client.py file
- you can also make changes to the server_address in the proxy.py file
- if you have problem with execution, Please check if you have all the packages mentioned 
  in the requirements file.
