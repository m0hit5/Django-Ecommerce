# About The Project
GreatKart is an eCommerce application built with Python Django Framework. Some of the features of this project includes custom user model, categories and products, Carts, Incrementing, Decrementing and removing car items, Unlimited Product image gallery, Orders, Payments, after-order functionalities such as reduce the quantify of sold products, send the order received email, clearing the cart, Order completion page as well as generating an invoice for the order. Also we have a Review and Rating system with the interactive rating stars that even allows you to rate a half-star rating. My account functionalities for the customer who can easily edit his profile, profile pictures, change his account password, and also manage his orders and much more. Finally hosted this application on AWS Elastic Beanstalk.

# Setup Instructions

1. Clone the repository `[git clone https://github.com/m0hit5/Django-Ecommerce.git]`
3. Navigrate to the working directory `cd greatkart-pre-deploy`
4. Open the project from the code editor `code .` or `atom .`
5. Create virtual environment `python -m venv env`
6. Activate the virtual environment `source env/Scripts/activate`
7. Install required packages to run the project `pip install -r requirements.txt`
8. Rename _.env-sample_ to _.env_
9. Fill up the environment variables:
    _Generate your own Secret key using this tool [https://djecrety.ir/](https://djecrety.ir/), copy and paste the secret key in the SECRET_KEY field._

    _Your configuration should look something like this:_
    ```sh
    SECRET_KEY=47d)n05#ei0rg4#)*@fuhc%$5+0n(t%jgxg$)!1pkegsi*l4c%
    DEBUG=True
    EMAIL_HOST=smtp.gmail.com
    EMAIL_PORT=587
    EMAIL_HOST_USER=youremailaddress@gmail.com
    EMAIL_HOST_PASSWORD=yourStrongPassword
    EMAIL_USE_TLS=True
    ```
    _Note: If you are using gmail account, make sure to [use app password](https://support.google.com/accounts/answer/185833)_
10. Create database tables
    ```sh
    python manage.py migrate
    ```
11. Create a super user
    ```sh
    python manage.py createsuperuser
    ```
    _GitBash users may have to run this to create a super user - `winpty python manage.py createsuperuser`_
12. Run server
    ```sh
    python manage.py runserver
    ```
13. Login to admin panel - (`http://127.0.0.1:8000/securelogin/`)
14. Add categories, products, add variations, register user, login, place orders and EXPLORE SO MANY FEATURES

