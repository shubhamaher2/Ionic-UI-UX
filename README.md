# Gold App FrontEnd  MObile App
To install and run an Ionic app locally from GitHub, you'll typically follow these steps:
#### This is Gold App BackEnd ###

###

1. **Clone the Repository**: First, clone the GitHub repository of the Ionic app to your local machine. You can do this using the ``git clone`` command. Navigate to the directory where you want to clone the repository and run:
2. 

   ```
   git clone (https://github.com/YOUR_USERNAMEs/Ionic-UI-UX.git)
   ```

   Replace `<YOUR_USERNAME>` with the actual URL of the GitHub repository.

3. **Install Dependencies**: Once you have cloned the repository, navigate into the directory of the cloned repository and install the necessary dependencies. Typically, Ionic apps use npm (Node Package Manager) for managing dependencies. Run the following command:

   ```
   npm install
   ```

   This will install all the required packages specified in the `package.json` file.

4. **Serve the App**: After installing the dependencies, you can serve the Ionic app locally using the Ionic CLI. Run the following command:

   ```
   ionic serve
   ```

   This command will start a local development server and open the Ionic app in your default web browser.

5. **View the App**: Once the server is up and running, you can view the Ionic app in your web browser by navigating to ``http://localhost:8100`` (by default, unless specified otherwise).

These steps assume that the Ionic app you're working with follows the typical structure and setup. If the repository contains any specific instructions or configurations, make sure to follow those as well. Additionally, ensure that you have Node.js and npm installed on your machine before proceeding with these steps.

Thank you !
## Backend Api 
####Login Api
getlogin 
```
/user/login?UPI=

```
```
body{
 email, password
}
```
Get States list
```
   getstates?count=100&name=ma&page=1
   ```
Get cities on the based on state 
```
   getcities?stateId= &count=100&name=ma&page=1
   ```
get rate of gold and silver from  Backend 
```
   /getrate
   ```

user onboard or signup

```
/subadmin/userOnboard
```
required data in body 
  mobileNumber,
    emailId,
    password,
    Name,
    userCityCode,
    userStateCode,
    userPincode,
    dateOfBirth,
    nomineeName,
    nomineeDateOfBirth,
    nomineeRelation,
    utmSource,
    utmMedium,
    utmCampaign,

    ```
     "mobileNumber":"90673433",
    "emailId":"ahers267@gmail.com",
    "password":"Shubham",
    "Name":"ShubhamAher",
    "userCityCode":"1GXDPyX2",
    "userStateCode":"ep9kJ7Px",
    "userPincode":"431113",
    "dateOfBirth":"2001-09-19",
    "nomineeName":"shather",
    "nomineeDateOfBirth":"2001-09-29",
    "nomineeRelation":"Brother",
    "utmSource":"FD",
    "utmMedium":"SA/BRANCH/MR/IFAPRIME/IFAGROWTH/NATIONALDISTRIBUTOR/CORPORATELIABILITIES",
    "utmCampaign":"EM42342434"
}
    ```


  ### get product list 
  ```
/user/getproductlist
```
###get product details

```
/user/proudct/info?productId=AU999GC20R
```
productId will be sku


## bank created 

```
/user/bank/bankcreate
```
JWt Required 
body data 
```
accountNumber,
    accountName,
    ifscCode
```


# buy / sell 
#### details of user 
```
/user/party/data ? dataType=

```
dataTpe should be { bank, his} bank de, his -> his of gold and silver ,and default you will get userdata 
```
{
    "event": "Succes",
    "gBalance": "10.000",
    "sBalance": "11.5000",
   
    "hist": [
        {
           
            "quantity": "2.0000",
            "totalAmount": "15505.17",
            "preTaxAmount": "15053.56",
            "metalType": "gold",
            "rate": "7526.78",
        
           
        }
        ,
       
        {
         
            "quantity": "1.0000",
            "totalAmount": "93.70",
            "preTaxAmount": "90.97",
            "metalType": "silver",
            "rate": "90.97",
           
            "userName": "ShubhamAher",
            "merchantTransactionId": "ahers287NaN",
            "mobileNumber": "9067343773",
            "goldBalance": "10.0000",
            "silverBalance": "6.0000",
            "totalTaxAmount": "2.73",
            "CGSTtaxPerc": "1.50",
            "CGSTtaxAmount": "1.36",
            "SGSTtaxPerc": "1.50",
            "SGSTtaxAmount": "1.36",
            "invoiceNumber": "SLP04254131",

        },
        
       
        
       
        
       
    ]
}
```
#### gold silver buy only 
```
/user/goldsilver/gSBuy
```
body
```
{
    "metalType":"SILVER/GOLD/SIP(SIP NOT Activated now)", "quantity":"0.5"
}
```

#### gold silver sell api
```
/user/goldsilver/gSSell
```
body should be
```
{
    "metalType":"SILVER/GOLD/SIP(SIP NOT Activated now)", "quantity":"0.5"
}

```

### user Bank Update 
API
```
/user/party/userBankUpdate
```
--body 
```
"accountNumber":"123456789012",
    "accountName":"Shubham",
    "ifscCode":"MAHB0001756"
```

#### product order on adre
Backed Api Should be integrate with aug
```
```

## integration of gold with our App
Login by VPA please send VPA as params 
```
```
** if user have buy gold with this app we will dont need signup
if not then just singup the user 
***
#### buy gold/ silver by amount 
amount should be send in parameter 

### we are not enabling to sell gold through our CCSA App
user will get creadiantial to login throw the gold app and he will able to see his histroy 
```
```
### new feature come in market 

### we are not enabling to sell gold through our CCSA App
user will get creadiantial to login throw the gold app and he will able to see his histroy 
```
```
### new feature come in market 
### we are not enabling to sell gold through our CCSA App
user will get creadiantial to login throw the gold app and he will able to see his histroy 
```
Log In Data from other match 
```



