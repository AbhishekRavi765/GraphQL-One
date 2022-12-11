# spring-boot-graphQL
GraphQL is a relatively new concept from Facebook that is billed as an alternative to REST for Web APIs


Readme
GraphQL

//Post req is used for get in graphql because of query in body

#####################################################

POST: localhost:8080/addPerson

Body:
[{ "id" : 11,
"name" : "abhishehk",
"mobile" : "9374809",
"email" : "abhi@gmail.com",
"address": [
"address1","address2","address3"
]
},
{ "id" : 21,
"name" : "abhi",
"mobile" : "12374809",
"email" : "abhishek@gmail.com",
"address": [
"address11","address22","address33"
]
}]

#####################################################

GET: localhost:8080/findAllPerson

#####################################################

POST: localhost:8080/getAll
Body:
    {
       getAllPerson
        { name,
          email,
          address
        }
    }

#####################################################

POST: localhost:8080/getPersonByEmail
Body:

	{
		findPerson(email :"abhi@gmail.com"){
			name
		}	
	}

#####################################################	