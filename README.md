Loan-Calculator
===============

Mini Project that uses the full stack. 

##Objectives
You'll create a really simple Angular app that calculates loan payment amounts based on an interest rate retrieved from a simple API that you'll also create.

##Step 1: Set up front end

We're going to set up our front end part of this app by having express fetch files and relay them to the client. We'll also make a really basic Angular app that will calcaulate payments for a loan.

* Use express's static middleware to serve a folder of static assets.
 * Create a folder called "public"
 * Move the index.html file already in the repo to the public folder. (Your index.html already has the markup you need.)
 * Move the styles.css to the public folder.
 * In the public folder, create a "js" folder.
 * In the js folder, create the following files:
 
```
public/js/app.js
public/js/controllers/main-ctrl.js
public/js/services/bank-service.js
```

 * Create a server.js file that serves the static files found in the "public" folder. Hint: `app.use(express.static(__dirname+'/public'));`

Verify that it's working by running your script, `node server.js` and opening the page in the browser, e.g. http://localhost:8080

##Step 2: Set up back end

* In server.js, create an endpoint that responds to a GET request on the `/interest_rate` route
* The interest_rate route should return a random number between .01 and .20, with two decimal places.
* Test your endpoint using Postman to make sure it returns the interest rate in a JSON object

##Step 3: Connect front end to back end

* Write the bank-service to include a method that returns a promise http call to retrieve the interest rate from your `/interest_rate` endpoint
* Have MainCtrl make the call and store the rate as `$scope.interest_rate`
* Run your app `node server.js` and make sure the interest rate shows
* Calculate the monthly payment of a loan defined at `$scope.principal` over 4 years (48 months) with the interest rate retrieved. Store the value as `$scope.monthly_payment`. Hint: use the basic formula for calculating the total loan amount with interest:

```
// P = Principal amount
// r = interest rate
// t = time (in years)

A = P*r*t

// A = total amount interest owed

A = P + (P*r*t)

// A = total amount owed with interest
```

## Copyright

© DevMountain LLC, 2016. Unauthorized use and/or duplication of this material without express and written permission from DevMountain, LLC is strictly prohibited. Excerpts and links may be used, provided that full and clear credit is given to DevMountain with appropriate and specific direction to the original content.

USA Web Cash( https://www.usawebcash.com/illinois-installment-loans ) is als working with us that is a payday loans provider company and you can get their services online. They helped us to create a loan calculator with Java coding and the code is described below:

// Display details of the loan
 
      System.out.println("Loan Amount: "+
         currencyFormat.format(loanAmount));
      System.out.println("Loan Term: "+
         termInYears+" years");
      System.out.println("Interest Rate: "+
         interestFormat.format(interestRate));
      System.out.println("Monthly Payment: "+
         currencyFormat.format(monthlyPayment));
 
   }
