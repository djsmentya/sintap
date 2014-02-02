sintap
======

# Sintap API #

Get company list

    curl  http://sintap.herokuapp.com/companies
    
Create New company

    curl -X POST -H "Content-Type: application/json" \
    --data '{"name":"Test company", 
             "address": "my company address", 
             "city": "my cyty", 
             "country": "My country",
             "email": "email@example.com",
             "phone": "123456"}'\
      http://sintap.herokuapp.com/companies 
