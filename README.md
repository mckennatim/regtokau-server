#heroctl server
This is the server for heated roof systems web control program
##weather apis
<a href="https://developer.forecast.io/">forecast.io</a>
user gmail, 6j,apikey: d374f89e74e135b440e7f786ca5fd857
### refs
http://stackoverflow.com/questions/8515872/simple-api-calls-with-node-js-and-express

http://stackoverflow.com/questions/5643321/how-to-make-remote-rest-call-inside-node-js-any-curl


#module/regtokau

Token authorization via APIkey. User registers with name and email and gets an apikey sent to their email address. Entering that apikey with your username returns a token which would is stored stored in the browser's localStorage. Protected areas on the server require an token to be sent with each request.

Allows Cross-Origin-Resource-Sharing (CORS). MongoDb stores records for each user containing (at least) name, email and apikey.

Uses node, express, passport and mongoose.

##config

Rename cfg-blank.js to cfg.js and fill out database, port, jwt secret and smtp mailer credentials.
    
    mv cfg-blank.js cfg.js

    npm install 

start mongod if not running

    monngod
the start server

    node server

test - from new console:

      mocha

