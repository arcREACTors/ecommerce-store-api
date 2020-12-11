Deployed Sites:

BackEnd- https://aqueous-brushlands-71762.herokuapp.com/ FrontEnd- https://arcreactors.github.io/Ecommerce-store-client/

Repos:

BackEnd- https://github.com/arcREACTors/ecommerce-store-api FrontEnd- https://github.com/arcREACTors/Ecommerce-store-client

SCRUM:
The Product:
An e-commerce store that sells your favorite memes using Stripe's safe and secure software to accept payment.

Members:
Master of Code - Tavish
Master of Darkness - Tristen
Master of Masters - Nick
Scrum Master - Alex


Planning/process/problem-solving strategy:
 Our planning was very fluid. We collectively broke down each prompt at the beginning and engaged each others interest for each in relation to how useful we thought it would be in the real world. We landed on the e-commerce store. Similar to project two, we wanted to complete the back end code first (for the most part) before tackling the front end in an attempt to simplify debugging and testing later. Each of us took either a schema and/or route, we later added two more schemas in similar fashion, and committed to github on the first day. After creating a repo for the front end we tried to deploy having issues with heroku. The second and third day, we separated the front end equally CRUDing the three resources with Tavish signing off on each of our codes before moving on. We worked as a team when problem-solving, debugging and testing with 4 sets of eyes on the code every day. This allowed us to correct syntax errors more rapidly but most importantly gave everyone a chance to share their thoughts on what the solution might be. Nick and Tristen took reigns connecting the store with Stripe. Our daily process, led by Alex, started with a recap on what we did the day prior and what we needed to do for that day. We typically tried to break the day into two parts (miniSprints), hopefully having something to cheer about over lunch and EOB. We tried to take mental breaks every 1-2 hours and get walk away from the screen. The team collaborated very well and everyone had a good amount of input.

Grow:
Taking more time at the very beginning to think through a lot of the issues we encountered. We tended to go back and forth to solve our issues towards the end, playing with the code instead of using algorithms. This could have been prevented with more upfront planning. Also our inexperience is a big factor and not fully understanding how everything works leading to us not properly structuring the project from the beginning. 

Glow:
Great collaboration, learned a lot through this process and how coding works within a team setting. 

WireFrames:
https://imgur.com/gallery/bOSaou9

ERD:

![Team Project - ECommerce](https://user-images.githubusercontent.com/71291178/101092119-20ad0880-3587-11eb-84ca-1083a442fd90.jpg)


#### Routes:
## AUTH
| Verb   | URI Pattern        | Controller#Action          |
|:-------|:----------------   |:------------------         |
| POST   | `/sign-up`         | `users#sign-up`            |
| POST   | `/sign-in`         | `users#sign-in`            |
| DELETE | `/sign-out`        | `users#sign-out`           |
| PATCH  | `/change-password` | `users#change-password`    |

## PRODUCTS
| Verb   | URI Pattern              | Controller#Action    |
|:-------|:----------------         |:------------------   |
| GET    | `/products`              | `products#index`     |
| GET    | `/products/:productId`   | `products#show`      |
| POST   | `/products`              | `products#create`    |

## PURCHASES
| Verb   | URI Pattern              | Controller#Action    |
|:-------|:-----------------        |:------------------   |
| POST   | `/purchases              | `purchases#create`   |
| GET    | `/purchases/:purchaseId` | `purchases#show`     |
| GET    | `/purchases              | `purchases#index`    |
| DELETE | `/purchases/:id`         | `purchases#delete`   |

## REVIEWS
| Verb   | URI Pattern                        | Controller#Action    |
|:-------|:-----------------                  |:------------------   |
| POST   | `/reviews/:productId               | `reviews#create`     |
| GET    | `/reviews/:reviewId/:productId`    | `reviews#show`       |
| DELETE | `/reviews/:reviewId/:productId`    | `reviews#delete`     |
| PATCH  | `/reviews/:reviewId/:productId`    | `reviews#patch`      |

List of Technologies:

JavaScript, React, Stripe, Express, MongoDB, Heroku, Mongoose

List of Unsolved Problems:

Styling, passing form data to Stripe, building a search feature for specific items

User Stories:
As an unregistered user, I would like to sign up with email and password so that I can upload items for sale.
As a registered user, I would like to sign in with email and password so I can access my uploaded items for sale.
As a signed in user, I would like to change password in order to keep my passwords updated and more secure.
As a signed in user, I would like to sign out so that no one else can access my items for sale.
As an unregistered user, I would like to see all of the products in order to survey products I might want to purchase.
As a signed in user, I would like to add and remove products from a shopping cart in case I change my mind about purchasing a product or want to purchase multiple products.
As a signed in user, I would like to purchase products in a shopping cart using Stripe in order to pay the vendor.
As a signed in user, I would like to see all my past orders so I can see what I don’t need to buy anymore.
