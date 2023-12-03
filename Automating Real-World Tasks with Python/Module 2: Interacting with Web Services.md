> RESTful APIs architecture, Flask & data serialization (tuần tự hóa dữ liệu), Python Requests Library, Diango

> complete a lab that uses Django to process text files with Python dictionaries and upload to a running web service
# Web Appliations and Services 
Web applications that have an API are also known as web services. Instead of browsing to a web page to type and click around, you can use your program to send a message known as an API call to the web service. The part of the program that listens on the network for API calls is called an API endpoint.

## RESTful APIs
- Unlike APIs which directly open up ports to the entire internet and directly connect, RESTful APIs rely on the HTTP protocol
- The HTTP protocol, in turn, can be further secured using HTTPS, and API endpoints can authenticate users via authorization tokens, API keys, or other security mechanisms. RESTful APIs use HTTP requests to perform CRUD (create, read, update, delete) operations on resources.

### RESTful methods
- HTTP request methods
- HTTP response status code

### JSON
- is a data-interchange format used in RESTful APIs to facilitate communication between clients and servers
- In RESTful services, JSON serves as the standard payload format for transmitting data
- When a client makes a request, the server processes it and sends back a response, often in JSON format.
  
## What is REST architecture?
- REST stands for Representational State Transfer
- REST architecture is an architectural style for designing networked applications and web services => standard way for clients and servers to communicate with each other over the internet.

> Key Takeaways:
> REST APIs are often designed to run on top of the HTTP protocol, utilizing standard HTTP features for communication.
> APIs are difficult to change after they are published and being utilized.

## Using REST APIs to access web data
> Think of APIs as a waiter at a restaurant. The waiter takes orders from the customer (front end). Then, the waiter communicates the order to the kitchen workers (back end) and comes back to the customer with their meal (API response).

- Key steps to access web data using RESTful APIs:
  + Identify the API endpoint
  + Select the appropriate HTTP method
  + Set up request headers
  + Prepare the request body
  + Send the HTTP request
  + Receive the HTTP response
  + Handle the response
  + Implement pagination and filtering (optional)
  + Authentication and authorization
  + Error handling
  + Rate limiting (if applicable)
  + Repeat as needed

## Python tools for REST APIs
### Client-side
- Requests: simplify sending HTTP requests, easy to use and has been around for a while.
  https://oxylabs.io/blog/httpx-vs-requests-vs-aiohttp
- PycURL: offers concurrent connections and can be much faster than Requests. Pycurl is more complicated to install than Requests, and it is not written in pure Python, which can make it harder to learn.

### Server-side
- Flask:
  + is a flexible and comfortable web development framework that is easy to set up and simple to use, which makes it good for beginners
  + handles requests sequentially
  + isn't good for high load needs
  + uses third-party modules, which can make it prone to security breaches
- Django:
  + is one of the most popular frameworks worldwide
  + free, open-source Python framework designed for building websites of any size, with any traffic needs
  + more secure than Flask, but Django software is much more unwieldy to work with
- FastAPI:
  + open-source, high-performing web framework for building web APIs in Python, and it includes hints similar to those in Python

# Python Requests



# Glossary terms from course 6, module 2
- **API endpoint:** The part of the program that listens on the network for API calls

- **Data serialization:** The process of taking an in-memory data structure, like a Python object, and turning it into something that can be stored on disk or transmitted across a network

- **Flask:** A Python library that makes it easier to create web applications and REST web services

- **JSON:** A data-interchange format used in RESTful APIs to facilitate communication between clients and servers

- **REST (Representational State Transfer):** Every request carries all the parameters and data needed for the server to satisfy that request

- **RESTful APIs:** Rely on the HTTP protocol, can be further secured using HTTPS, and API endpoints can authenticate users via authorization tokens, API keys, or other security mechanisms

- **REST architecture:** An architectural style for designing networked applications and web services

- **Richardson Maturity Model (RMM):** A framework that categorizes and describes different levels of implementation for RESTful APIs based on their adherence to the six constraints

- **Web application:** An application that you interact with over HTTP


# Project: Process Text Files with Python Dictionaries and Upload to Running Web Service
