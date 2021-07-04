# UserOrderProduct

## Step to run the User, Order and Product services
1. Download AxonServer [AxonServer](https://axoniq.io/product-overview/axon-server)
2. Run ```java -jar axonserver.jar```.
3. Run **ServiceRegistry** project.
4. Build **core** Project.
5. Add **core** depedency in **OrdersService**, **ProductsService**, **UsersService** service ans build.
6. Run all services (**OrdersService**, **ProductsService** and **UsersService**).
7. Open [ServiceRegistry](http://localhost:8761/) and [AxonServer](http://localhost:8024/)
8. CURL:
          curl -H "Content-Type: application/json" -X GET http://localhost:51458/users/27b95829-4f3f-4ddf-8983-151ba010e35b/payment-details

          curl -d '{"title":"Mouse","price":500,"quantity":"5"}' -H "Content-Type: application/json" -X POST http://localhost:60632/products
          curl -d '{"title":"Monitor","price":5000,"quantity":"5"}' -H "Content-Type: application/json" -X POST http://localhost:60632/products
          curl -d '{"title":"Keyboard","price":1500,"quantity":"5"}' -H "Content-Type: application/json" -X POST http://localhost:60632/products
          curl -H "Content-Type: application/json" -X GET http://localhost:60632/products

          curl -d '{"quantity":2,"addressId":"River Residency","productId":"2c980696-f99a-4d61-9802-d354a05144ab"}' -H "Content-Type: application/json" -X POST http://localhost:55133/orders





          
