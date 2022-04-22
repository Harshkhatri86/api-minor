from flask import Flask
import json
import jsonify
app  = Flask(__name__)
data ={
    "orders": [{
            "order_number": "N12345678",
            "order_description": "1 Carton of water",
            "weight": "500g",
            "quantity": "1",
            "pickup_date": "10/1/21",
            "pickup_address_line_1": "123 Raffles Place",
            "pickup_address_line_2": "",
            "pickup_postal_code": "101111",
            "delivery_date": "11/01/2021",
            "delivery_address_line_1": "123 City Hall",
            "delivery_address_line_2": "",
            "delivery_postal_code": "546090",
            "customer_first_name": "Aaron 1",
            "customer_last_name": "Lo",
            "customer_email": "aaron.lo@mail.com",
            "customer_phone_number": "12345678",
            "customer_company": "",
            "merchant_name": "Merchant 1",
            "approval_status": "not_picked_up"
        },
        {
            "order_number": "N12345679",
            "order_description": "1 Carton of water",
            "weight": "500g",
            "quantity": "1",
            "pickup_date": "10/1/21",
            "pickup_address_line_1": "123 Raffles Place",
            "pickup_address_line_2": "",
            "pickup_postal_code": "101111",
            "delivery_date": "11/01/2021",
            "delivery_address_line_1": "123 City Hall",
            "delivery_address_line_2": "",
            "delivery_postal_code": "546090",
            "customer_first_name": "Aaron 1",
            "customer_last_name": "Lo",
            "customer_email": "aaron.lo@mail.com",
            "customer_phone_number": "12345678",
            "customer_company": "",
            "merchant_name": "Merchant 1",
            "approval_status": "not_picked_up"
        },
        {
            "order_number": "N12345680",
            "order_description": "1 Carton of water",
            "weight": "500g",
            "quantity": "1",
            "pickup_date": "10/1/21",
            "pickup_address_line_1": "123 Raffles Place",
            "pickup_address_line_2": "",
            "pickup_postal_code": "101111",
            "delivery_date": "11/01/2021",
            "delivery_address_line_1": "123 City Hall",
            "delivery_address_line_2": "",
            "delivery_postal_code": "546090",
            "customer_first_name": "Aaron 1",
            "customer_last_name": "Lo",
            "customer_email": "aaron.lo@mail.com",
            "customer_phone_number": "12345678",
            "customer_company": "",
            "merchant_name": "Merchant 1",
            "approval_status": "not_picked_up"
        },
        {
            "order_number": "N12345681",
            "order_description": "1 Carton of water",
            "weight": "500g",
            "quantity": "1",
            "pickup_date": "10/1/21",
            "pickup_address_line_1": "123 Raffles Place",
            "pickup_address_line_2": "",
            "pickup_postal_code": "101111",
            "delivery_date": "11/01/2021",
            "delivery_address_line_1": "123 City Hall",
            "delivery_address_line_2": "",
            "delivery_postal_code": "546090",
            "customer_first_name": "Aaron 1",
            "customer_last_name": "Lo",
            "customer_email": "aaron.lo@mail.com",
            "customer_phone_number": "12345678",
            "customer_company": "",
            "merchant_name": "Merchant 1",
            "approval_status": "not_picked_up"
        },
        {
            "order_number": "N12345682",
            "order_description": "1 Carton of water",
            "weight": "500g",
            "quantity": "1",
            "pickup_date": "10/1/21",
            "pickup_address_line_1": "123 Raffles Place",
            "pickup_address_line_2": "",
            "pickup_postal_code": "101111",
            "delivery_date": "11/01/2021",
            "delivery_address_line_1": "123 City Hall",
            "delivery_address_line_2": "",
            "delivery_postal_code": "546090",
            "customer_first_name": "Aaron 1",
            "customer_last_name": "Lo",
            "customer_email": "aaron.lo@mail.com",
            "customer_phone_number": "12345678",
            "customer_company": "",
            "merchant_name": "Merchant 1",
            "approval_status": "not_picked_up"
        },
        {
            "order_number": "N12345683",
            "order_description": "1 Carton of water",
            "weight": "500g",
            "quantity": "1",
            "pickup_date": "10/1/21",
            "pickup_address_line_1": "123 Raffles Place",
            "pickup_address_line_2": "",
            "pickup_postal_code": "101111",
            "delivery_date": "11/01/2021",
            "delivery_address_line_1": "123 City Hall",
            "delivery_address_line_2": "",
            "delivery_postal_code": "546090",
            "customer_first_name": "Aaron 1",
            "customer_last_name": "Lo",
            "customer_email": "aaron.lo@mail.com",
            "customer_phone_number": "12345678",
            "customer_company": "",
            "merchant_name": "Merchant 1",
            "approval_status": "not_picked_up"
        },
        {
            "order_number": "N12345684",
            "order_description": "1 Carton of water",
            "weight": "500g",
            "quantity": "1",
            "pickup_date": "10/1/21",
            "pickup_address_line_1": "123 Raffles Place",
            "pickup_address_line_2": "",
            "pickup_postal_code": "101111",
            "delivery_date": "11/01/2021",
            "delivery_address_line_1": "123 City Hall",
            "delivery_address_line_2": "",
            "delivery_postal_code": "546090",
            "customer_first_name": "Aaron 1",
            "customer_last_name": "Lo",
            "customer_email": "aaron.lo@mail.com",
            "customer_phone_number": "12345678",
            "customer_company": "",
            "merchant_name": "Merchant 1",
            "approval_status": "not_picked_up"
        },
        {
            "order_number": "N12345685",
            "order_description": "1 Carton of water",
            "weight": "500g",
            "quantity": "1",
            "pickup_date": "10/1/21",
            "pickup_address_line_1": "123 Raffles Place",
            "pickup_address_line_2": "",
            "pickup_postal_code": "101111",
            "delivery_date": "11/01/2021",
            "delivery_address_line_1": "123 City Hall",
            "delivery_address_line_2": "",
            "delivery_postal_code": "546090",
            "customer_first_name": "Aaron 1",
            "customer_last_name": "Lo",
            "customer_email": "aaron.lo@mail.com",
            "customer_phone_number": "12345678",
            "customer_company": "",
            "merchant_name": "Merchant 1",
            "approval_status": "not_picked_up"
        },
        {
            "order_number": "N12345686",
            "order_description": "1 Carton of water",
            "weight": "500g",
            "quantity": "1",
            "pickup_date": "10/1/21",
            "pickup_address_line_1": "123 Raffles Place",
            "pickup_address_line_2": "",
            "pickup_postal_code": "101111",
            "delivery_date": "11/01/2021",
            "delivery_address_line_1": "123 City Hall",
            "delivery_address_line_2": "",
            "delivery_postal_code": "546090",
            "customer_first_name": "Aaron 1",
            "customer_last_name": "Lo",
            "customer_email": "aaron.lo@mail.com",
            "customer_phone_number": "12345678",
            "customer_company": "",
            "merchant_name": "Merchant 1",
            "approval_status": "not_picked_up"
        },
        {
            "order_number": "N12345687",
            "order_description": "1 Carton of water",
            "weight": "500g",
            "quantity": "1",
            "pickup_date": "10/1/21",
            "pickup_address_line_1": "123 Raffles Place",
            "pickup_address_line_2": "",
            "pickup_postal_code": "101111",
            "delivery_date": "11/01/2021",
            "delivery_address_line_1": "123 City Hall",
            "delivery_address_line_2": "",
            "delivery_postal_code": "546090",
            "customer_first_name": "Aaron 1",
            "customer_last_name": "Lo",
            "customer_email": "aaron.lo@mail.com",
            "customer_phone_number": "12345678",
            "customer_company": "",
            "merchant_name": "Merchant 1",
            "approval_status": "not_picked_up"
        },
        {
            "order_number": "N12345688",
            "order_description": "1 Carton of water",
            "weight": "500g",
            "quantity": "1",
            "pickup_date": "10/1/21",
            "pickup_address_line_1": "123 Raffles Place",
            "pickup_address_line_2": "",
            "pickup_postal_code": "101111",
            "delivery_date": "11/01/2021",
            "delivery_address_line_1": "123 City Hall",
            "delivery_address_line_2": "",
            "delivery_postal_code": "546090",
            "customer_first_name": "Aaron 1",
            "customer_last_name": "Lo",
            "customer_email": "aaron.lo@mail.com",
            "customer_phone_number": "12345678",
            "customer_company": "",
            "merchant_name": "Merchant 1",
            "approval_status": "not_picked_up"
        },
        {
            "order_number": "N12345689",
            "order_description": "1 Carton of water",
            "weight": "500g",
            "quantity": "1",
            "pickup_date": "10/1/21",
            "pickup_address_line_1": "123 Raffles Place",
            "pickup_address_line_2": "",
            "pickup_postal_code": "101111",
            "delivery_date": "11/01/2021",
            "delivery_address_line_1": "123 City Hall",
            "delivery_address_line_2": "",
            "delivery_postal_code": "546090",
            "customer_first_name": "Aaron 1",
            "customer_last_name": "Lo",
            "customer_email": "aaron.lo@mail.com",
            "customer_phone_number": "12345678",
            "customer_company": "",
            "merchant_name": "Merchant 1",
            "approval_status": "not_picked_up"
        },
        {
            "order_number": "N12345690",
            "order_description": "1 Carton of water",
            "weight": "500g",
            "quantity": "1",
            "pickup_date": "10/1/21",
            "pickup_address_line_1": "123 Raffles Place",
            "pickup_address_line_2": "",
            "pickup_postal_code": "101111",
            "delivery_date": "11/01/2021",
            "delivery_address_line_1": "123 City Hall",
            "delivery_address_line_2": "",
            "delivery_postal_code": "546090",
            "customer_first_name": "Aaron 1",
            "customer_last_name": "Lo",
            "customer_email": "aaron.lo@mail.com",
            "customer_phone_number": "12345678",
            "customer_company": "",
            "merchant_name": "Merchant 1",
            "approval_status": "not_picked_up"
        },
        {
            "order_number": "N12345691",
            "order_description": "1 Carton of water",
            "weight": "500g",
            "quantity": "1",
            "pickup_date": "10/1/21",
            "pickup_address_line_1": "123 Raffles Place",
            "pickup_address_line_2": "",
            "pickup_postal_code": "101111",
            "delivery_date": "11/01/2021",
            "delivery_address_line_1": "123 City Hall",
            "delivery_address_line_2": "",
            "delivery_postal_code": "546090",
            "customer_first_name": "Aaron 1",
            "customer_last_name": "Lo",
            "customer_email": "aaron.lo@mail.com",
            "customer_phone_number": "12345678",
            "customer_company": "",
            "merchant_name": "Merchant 1",
            "approval_status": "not_picked_up"
        },
        {
            "order_number": "N12345692",
            "order_description": "1 Carton of water",
            "weight": "500g",
            "quantity": "1",
            "pickup_date": "10/1/21",
            "pickup_address_line_1": "123 Raffles Place",
            "pickup_address_line_2": "",
            "pickup_postal_code": "101111",
            "delivery_date": "11/01/2021",
            "delivery_address_line_1": "123 City Hall",
            "delivery_address_line_2": "",
            "delivery_postal_code": "546090",
            "customer_first_name": "Aaron 1",
            "customer_last_name": "Lo",
            "customer_email": "aaron.lo@mail.com",
            "customer_phone_number": "12345678",
            "customer_company": "",
            "merchant_name": "Merchant 1",
            "approval_status": "not_picked_up"
        },
        {
            "order_number": "N12345693",
            "order_description": "1 Carton of water",
            "weight": "500g",
            "quantity": "1",
            "pickup_date": "10/1/21",
            "pickup_address_line_1": "123 Raffles Place",
            "pickup_address_line_2": "",
            "pickup_postal_code": "101111",
            "delivery_date": "11/01/2021",
            "delivery_address_line_1": "123 City Hall",
            "delivery_address_line_2": "",
            "delivery_postal_code": "546090",
            "customer_first_name": "Aaron 1",
            "customer_last_name": "Lo",
            "customer_email": "aaron.lo@mail.com",
            "customer_phone_number": "12345678",
            "customer_company": "",
            "merchant_name": "Merchant 1",
            "approval_status": "not_picked_up"
        },
        {
            "order_number": "N12345694",
            "order_description": "1 Carton of water",
            "weight": "500g",
            "quantity": "1",
            "pickup_date": "10/1/21",
            "pickup_address_line_1": "123 Raffles Place",
            "pickup_address_line_2": "",
            "pickup_postal_code": "101111",
            "delivery_date": "11/01/2021",
            "delivery_address_line_1": "123 City Hall",
            "delivery_address_line_2": "",
            "delivery_postal_code": "546090",
            "customer_first_name": "Aaron 1",
            "customer_last_name": "Lo",
            "customer_email": "aaron.lo@mail.com",
            "customer_phone_number": "12345678",
            "customer_company": "",
            "merchant_name": "Merchant 1",
            "approval_status": "not_picked_up"
        },
        {
            "order_number": "N12345695",
            "order_description": "1 Carton of water",
            "weight": "500g",
            "quantity": "1",
            "pickup_date": "10/1/21",
            "pickup_address_line_1": "123 Raffles Place",
            "pickup_address_line_2": "",
            "pickup_postal_code": "101111",
            "delivery_date": "11/01/2021",
            "delivery_address_line_1": "123 City Hall",
            "delivery_address_line_2": "",
            "delivery_postal_code": "546090",
            "customer_first_name": "Aaron 1",
            "customer_last_name": "Lo",
            "customer_email": "aaron.lo@mail.com",
            "customer_phone_number": "12345678",
            "customer_company": "",
            "merchant_name": "Merchant 1",
            "approval_status": "not_picked_up"
        },
        {
            "order_number": "N12345696",
            "order_description": "1 Carton of water",
            "weight": "500g",
            "quantity": "1",
            "pickup_date": "10/1/21",
            "pickup_address_line_1": "123 Raffles Place",
            "pickup_address_line_2": "",
            "pickup_postal_code": "101111",
            "delivery_date": "11/01/2021",
            "delivery_address_line_1": "123 City Hall",
            "delivery_address_line_2": "",
            "delivery_postal_code": "546090",
            "customer_first_name": "Aaron 1",
            "customer_last_name": "Lo",
            "customer_email": "aaron.lo@mail.com",
            "customer_phone_number": "12345678",
            "customer_company": "",
            "merchant_name": "Merchant 1",
            "approval_status": "not_picked_up"
        },
        {
            "order_number": "N12345697",
            "order_description": "1 Carton of water",
            "weight": "500g",
            "quantity": "1",
            "pickup_date": "10/1/21",
            "pickup_address_line_1": "123 Raffles Place",
            "pickup_address_line_2": "",
            "pickup_postal_code": "101111",
            "delivery_date": "11/01/2021",
            "delivery_address_line_1": "123 City Hall",
            "delivery_address_line_2": "",
            "delivery_postal_code": "546090",
            "customer_first_name": "Aaron 1",
            "customer_last_name": "Lo",
            "customer_email": "aaron.lo@mail.com",
            "customer_phone_number": "12345678",
            "customer_company": "",
            "merchant_name": "Merchant 1",
            "approval_status": "not_picked_up"
        },
        {
            "order_number": "N12345698",
            "order_description": "1 Carton of water",
            "weight": "500g",
            "quantity": "1",
            "pickup_date": "10/1/21",
            "pickup_address_line_1": "123 Raffles Place",
            "pickup_address_line_2": "",
            "pickup_postal_code": "101111",
            "delivery_date": "11/01/2021",
            "delivery_address_line_1": "123 City Hall",
            "delivery_address_line_2": "",
            "delivery_postal_code": "546090",
            "customer_first_name": "Aaron 1",
            "customer_last_name": "Lo",
            "customer_email": "aaron.lo@mail.com",
            "customer_phone_number": "12345678",
            "customer_company": "",
            "merchant_name": "Merchant 1",
            "approval_status": "not_picked_up"
        },
        {
            "order_number": "N12345699",
            "order_description": "1 Carton of water",
            "weight": "500g",
            "quantity": "1",
            "pickup_date": "10/1/21",
            "pickup_address_line_1": "123 Raffles Place",
            "pickup_address_line_2": "",
            "pickup_postal_code": "101111",
            "delivery_date": "11/01/2021",
            "delivery_address_line_1": "123 City Hall",
            "delivery_address_line_2": "",
            "delivery_postal_code": "546090",
            "customer_first_name": "Aaron 1",
            "customer_last_name": "Lo",
            "customer_email": "aaron.lo@mail.com",
            "customer_phone_number": "12345678",
            "customer_company": "",
            "merchant_name": "Merchant 1",
            "approval_status": "not_picked_up"
        }
    ]
}
@app.route('/',methods= ["GET"])


def beckend():
    return data

if __name__=='__main__':
    app.run(debug=True)
