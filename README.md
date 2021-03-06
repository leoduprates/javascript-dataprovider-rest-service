# javascript-dataprovider-rest-service

Dataprovider developed in REST service for use in automated and performance testing.

This sample expose fake data generated by package [faker.js](https://github.com/marak/Faker.js/) in JSON or CSV format.

Use [ExpressJS](https://expressjs.com/pt-br/), [consign](https://www.npmjs.com/package/consign) and [body-parser](https://www.npmjs.com/package/body-parser) to implement the rest service.

About Unit Tests, use [mochajs](https://mochajs.org/) and [chaijs](https://www.chaijs.com/) to implement automation tests for api.

## GET 

**JSON Request:** 
```
http://{YOUR_URL}/dataprovider?format=json&property=firstName,lastName&quantity=1
```

**JSON Response:**
```
[
    {
        "firstName": "Yago",
        "lastName": "Barros"
    }
]
```

**XML Request:**
```
http://localhost:3000/dataprovider?format=csv&property=firstName,lastName&quantity=1
```

**XML Response:**
```
"firstName","lastName"
"Bruna","Macedo"
```

**Property Options:**
- firstName
- lastName
- fullName
- jobTitle
- prefix
- suffix
- title
- jobDescriptor
- jobArea
- jobType
- phoneNumber
- phoneNumberFormat
- phoneFormats
- zipCode
- city
- cityPrefix
- citySuffix
- streetName
- streetAddress
- streetSuffix
- streetPrefix
- secondaryAddress
- county
- country
- countryCode
- state
- stateAbbr
- latitude
- longitude
- past
- future
- between
- recent
- month
- weekday
- account
- accountName
- mask
- amount
- transactionType
- currencyCode
- currencyName
- currencySymbol
- bitcoinAddress
- iban
- bic
- avatar
- email
- exampleEmail
- userName
- protocol
- url
- domainName
- domainSuffix
- domainWord
- ip
- ipv6
- userAgent
- color
- mac
- password
- word
- words
- sentence
- slug
- sentences
- paragraph
- paragraphs
- text
- lines
- number
- arrayElement
- objectElement
- uuid
- boolean
- word
- words
- image
- locale
- alphaNumeric
- fileName
- commonFileName
- mimeType
- commonFileType
- commonFileExt
- fileType
- fileExt
- directoryPath
- filePath
- barcodeSantander
- barcodeBradesco


### Setup

1. Global Dependencies

* Install [NODE](https://nodejs.org/en/)

* Install **NODEMON**
```
$ npm install --global nodemon
```

2. Dependencies

* Install npm packages
```
$ npm install
```    

### Start Service

* NPM:
```
npm start
```

### Start Unit Tests

* NPM:
```
npm test
```


### Resources

##### [NodeJS](https://nodejs.org/en/)
##### [ExpressJS](https://expressjs.com/pt-br/)
##### [faker.js](https://github.com/marak/Faker.js/) 
##### [consign](https://www.npmjs.com/package/consign)
##### [body-parser](https://www.npmjs.com/package/body-parser)
##### [mochajs](https://mochajs.org/)
##### [chaijs](https://www.chaijs.com/)
