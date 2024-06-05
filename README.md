# Product Processor
You have an array of products, and you need to write a function that:

1. Filters out the products that are out of stock.
2. Calculates the total value of each product in stock (price * quantity).
3. Applies a discount to the total value of products that belong to a specific category.
4. Formats and returns the final array to include only the product name, category, and the discounted total value. Match the output format from the example below.

Example output:

```javascript
[
  { name: "Laptop", category: "Electronics", discountedTotalValue: "5000.00" },
  { name: "Shirt", category: "Apparel", discountedTotalValue: "1800.00" },
  { name: "Jeans", category: "Apparel", discountedTotalValue: "1800.00" },
  { name: "TV", category: "Electronics", discountedTotalValue: "4500.00" },
  { name: "Hat", category: "Apparel", discountedTotalValue: "2700.00" }
]
```

Starter code:

JS:

```javascript
const startProcessing = () => {
  const products = [
    {
      name: "Laptop",
      category: "Electronics",
      price: 1000,
      quantity: 5,
      inStock: true,
    },
    {
      name: "Phone",
      category: "Electronics",
      price: 500,
      quantity: 0,
      inStock: false,
    },
    {
      name: "Shirt",
      category: "Apparel",
      price: 20,
      quantity: 100,
      inStock: true,
    },
    {
      name: "Jeans",
      category: "Apparel",
      price: 40,
      quantity: 50,
      inStock: true,
    },
    {
      name: "TV",
      category: "Electronics",
      price: 1500,
      quantity: 3,
      inStock: true,
    },
    {
      name: "Hat",
      category: "Apparel",
      price: 15,
      quantity: 200,
      inStock: true,
    },
  ];

  const discountCategory = "Apparel";
  const discountRate = 0.1; // 10% discount
  console.log(processProducts(products, discountCategory, discountRate));
};

const processProducts = (products, discountCategory, discountRate) => {
  // Your code goes here
};
```

Submission
Submit a link to a repository that has HTML, CSS, and JavaScript.