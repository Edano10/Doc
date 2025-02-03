## Paaystack documentation
   Save Organization Pay stack Credential (Method =POST)
  		http://127.0.0.1:addyourort/paystack
           {
    	     "paystack_key":"add the paystack key here"
           }


    
    Get Organization Pay Stack Credential (Method =GET)
      http://127.0.0.1:addyourport/paystack_credentials

             {
    	          "message": "Paystack credentials not found"
             }



       Check Organization Paystack Balance (Method= GET)
        
         http://127.0.0.1:addyourport/paystack/balance
                 {
                  "Current Balance": {
                      "data": [
                          {
                              "balance": 0,
                              "currency": "NGN"
                          }
                      ],
                      "message": "Balances retrieved",
                      "status": true
                  }
              }



   List all approved bank that the organization can use (Method=GET)
    http://127.0.0.1:addyourport/paystack/bank

     {
      "Banks": {
          "data": [
                {
                  "active": true,
                  "code": "120001",
                  "country": "Nigeria",
                  "createdAt": "2022-05-31T06:50:27.000Z",
                  "currency": "NGN",
                  "gateway": "",
                  "id": 302,
                  "is_deleted": false,
                  "longcode": "120001",
                  "name": "9mobile 9Payment Service Bank",
                  "pay_with_bank": false,
                  "slug": "9mobile-9payment-service-bank-ng",
                  "supports_transfer": true,
                  "type": "nuban",
                  "updatedAt": "2022-06-23T09:33:55.000Z"
              },
              {
                  "active": true,
                  "code": "404",
                  "country": "Nigeria",
                  "createdAt": "2020-12-07T16:19:09.000Z",
                  "currency": "NGN",
                  "gateway": null,
                  "id": 174,
                  "is_deleted": false,
                  "longcode": "",
                  "name": "Abbey Mortgage Bank",
                  "pay_with_bank": false,
                  "slug": "abbey-mortgage-bank-ng",
                  "supports_transfer": true,
                  "type": "nuban",
                  "updatedAt": "2023-09-14T13:02:38.000Z"
          },
             }
          ],
          "message": "Banks retrieved",
          "status": true
      }
  }


List all transaction history (Method =GET)
http://127.0.0.1:addyourport/paystack/employees/transaction_history


Delete Organization paystack credential( Method=DELETE)
      
    http://127.0.0.1:addyourport/paystack/employee_id
		 {
    		"message": "Paystack Credentials data deleted successfully"
     }


 Initiate  employee transaction (Method = POST)
		 http://127.0.0.1:addyourport/paystack/employees/rep_code
      
      [
        {"employee_id": 1},
        {"employee_id": 2}
      ]

  



          


              

