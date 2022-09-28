// 1)What are the different types of HTTP requests?
// Ans->The most commonly used HTTP request methods are GET, POST, PUT, PATCH, and DELETE.
       There are also crud operators like read,write,sendetc


// 2)Explain the concept of middleware in Node.js.
// Ans->Middleware is a request handler that has access to the application's request-response cycle.It takes three parameters req,res and next.next is used to execute the next middleware if present else it will ask the router to send response to the client.If we will not write next()then respose will be not sent and the browser will be refreshing again and again.It will not stop.There are two type of middleware
// i)Local middleware->It will be applied to only routes in which we will mention it.
   eg:const localMiddleware=(req,res,next)=>{
    console.log("hi i am localmiddleware);
    next();

   }
// ii)Global middleware->It will be applied to all routes 
  eg:app.use(cors())

// 3) Explain CORS
// Ans->CORS stands for cross origin resounce sharing.It is basically it run the two port numbers and run on the browsers.it is kind of policy for stopping the sharing the data of two servers.Our server will like to share it resource only with those clients who are in same domain.By using cors globaly it allow our server to share data with clients who are not in same domain by relax the security applied to the API.


// 4)What is Express. how it helps you to create a backend application
// Ans->Express is Fast, unopinionated, minimalist web framework for Nodejs.It provides broad features for building web and mobile applications. It is used to build a single page, multipage web application

// 5)Explain min 5 status codes gets used in Backend development
// Ans->Informational responses (100–199)
        Successful responses (200–299)
        Redirection messages (300–399)
        Client error responses (400–499)
        Server error responses (500–599)

// 6)Difference between HTTP and HTTPS
// Ans->HTTP stands for HyperText Transfer Protocol and HTTPS stands for HyperText Transfer Protocol Secure.
// In HTTP, URL begins with “http://” whereas URL starts with “https://”
// HTTP uses port number 80 for communication and HTTPS uses 443
// HTTP is considered to be insecure and HTTPS is secure
// HTTP Works at Application Layer and HTTPS works at Transport Layer
// HTTP does not require any certificates and HTTPS needs SSL Certificates
// HTTP speed is faster than HTTPS and HTTPS speed is slower than HTTP