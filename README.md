# GraphQL_Restaurant_Data

In this project you can experiment with GraphQL queries and mutation


install :
npm i express express-graphql graphql
npx create-strapi-app my-project –quickstart

port:
http://localhost:5501/graphql


Examples:
1) QUERY
{ restaurants{
  id
  name
  description
  dishes {
    name
    price
  }
}}




2) MUTATION 
mutation setrestaurants {
  setrestaurant(input: {
    name: "Marco Polo",
    description: "Fish",
  }) {
    name
    description
  }
}

