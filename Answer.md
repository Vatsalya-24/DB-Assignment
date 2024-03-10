Answer 1

1. The relationship between the "Product" and "Product_Category" is a one-to-many relationship, where one product belongs to one category, but one category can have multiple products.
2. In the "Product" , "category_id" act as a foreign key referencing the "id" in the "Product_Category" table.

Answer 2

1. Use the foreign key constraint between the "Product":"category_id" and "Product_Category":"id" to ensures that every value in the "category_id" of the "Product" must match an existing "id" in the "Product_Category".
2. Any attempt to insert or update a "product" with an invalid "category_id" will result in error, preventing the operation from being completed.
"FOREIGN KEY (category_id) REFERENCES Product_Category(id)" we can use this query to add the above feature.