sintap
======

# Sintap API #

### Get company list

    curl  http://sintap.herokuapp.com/companies

Result Example: 

    [{
        "_id":"52ee5b76582aeee36d000001",
        "name": "My company",
        "address":"my address",
        "city":"mycyty",
        "country":null,
        "email":null,
        "phone":null
     },
     {
        "_id":"52ee5b76582aeee36d000001",
        "name": "My second company",
        "address":"my address",
        "city":"my cyty",
        "country":null,
        "email":null,
        "phone":null
     }]
     
     
### Create New company

    curl -X POST -H "Content-Type: application/json" \
    --data '{"name":"Test company", 
             "address": "my company address", 
             "city": "my cyty", 
             "country": "My country",
             "email": "email@example.com",
             "phone": "123456"}'\
      http://sintap.herokuapp.com/companies 
      
### Update company

    curl -X PUT -H "Content-Type: application/json" \
    --data '{"name":"New company", 
             "address": "New company address", 
             "city": "New cyty", 
             "country": "New country",
             "email": "new_email@example.com",
             "phone": "123456"}'\
    http://sintap.herokuapp.com/companies/:company_id

### Get company details
    
    curl  http://sintap.herokuapp.com/companies/:company_id
    
Result Example: 

    {
        "_id":"52ee5b76582aeee36d000001",
        "address":"my address",
        "city":"mycyty",
        "country":null,
        "email":null,
        "name": "My company",
        "phone":null
     }
    
