# Heady-Product
npm init

npm start

# Apis 
# Categeroies

Create Categories and sub categories
POST  http://localhost:3000/api/categories

{
    "categoryName": "Furniture",
    "childCategories": [
        {
            "categoryName": "Fchair",
            "childCategories": [
                {
                    "categoryName": "CHstool"
                },
                {
                    "categoryName": "CHoffice"
                }
            ]
        },
        {
            "categoryName": "Ftable",
            "childCategories": [
                {
                    "categoryName": "TBWood"
                },
                {
                    "categoryName": "TBsteel"
                }
            ]
        }
    ]
}

Get All Categories
GET   http://localhost:3000/api/categories

Get Category By Id
GET   http://localhost:3000/api/categories/{id}

# Products

Create Products with multiple categories
POST  http://localhost:3000/api/products
Payload 
{
    "productName" : "Samsung",
    "price" : 1468,
    "categories":[
        {
            "_id": "5f2ae83eb08e5835141a8f6e",
            "categoryName": "SmartPhones"
        },
        {
            "_id": "5f2ae83eb08e5835141a8f6e",
            "categoryName": "Phones"
        }
    ]
}

Get All Products
GET   http://localhost:3000/api/products

Get All Products By Categories
GET   http://localhost:3000/api/products?category={id}

Get Product By Id
GET   http://localhost:3000/api/products/{id}

Update Product By Id
GET   http://localhost:3000/api/products/{id}

delete Product By Id
GET   http://localhost:3000/api/products/{id}



