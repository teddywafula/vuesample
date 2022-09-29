<template>
    <div id="page-wrap">
      <ProductsGrid :products="products" />
    </div>
  </template>
  
  <script>
    // import axios from 'axios';
    import { products } from '../fake-data';
    import ProductsGrid from '../components/ProductsGrid';
    
    export default {
        name: "ProductsPage",
        data() {
            return {
                products: products,
            };
        },
        // async created() {
        //     const result = await axios.get(
        //         'http://localhost:8000/api/products/',
        //         {
        //             headers: {
        //                 'Access-Control-Allow-Origin': '*',
        //             }
        //         }
        //         );
        //     const products = result.data;
        //     this.products = products;
        // },
        components: { ProductsGrid }
    };
  </script>
  

  