
# About The Project
So my cousin just open a wears company where she sells all kinds of wears for adults and children, so I thought it would be good place to develop an E-commerce application for her to manage her company. This is a Robust E-commerce application that you can use as a prototype for your E-commerce applications.  

<img src="https://github.com/fegorstar/mobhil-web/blob/master/mobhil/static/img/homepage.PNG">


## App Features
- Store: Which consists of the lists of products
- Carts: consist of products selected by customers for purchase
- Accounts: Which allows the users to register and login.
- Search functionality and Pangination
- Orders: Which consists lists of order made by customers.
- Category: which consists of category of products in store
- Payment Gateway Integration- Paypal/Stripe
- Review and Rating System 


# Setup Instructions
1. Clone the repository `git clone https://github.com/fegorstar/fegoshop.git`
2. Navigrate to the working directory `cd fegoshop`
3. Open the project from the code editor `code .` or `atom .`
4. Create virtual environment `virtualenv venv`
5. Activate the virtual environment `source venv/Scripts/activate`
6. Install required packages to run the project `pip install -r requirements.txt`
7. Rename _.env-sample_ to _.env_
8. Fill up the environment variables:
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
9. Create database tables
    ```sh
    python manage.py migrate
    ```
10. Create a super user
    ```sh
    python manage.py createsuperuser
    ```
    _GitBash users may have to run this to create a super user - `winpty python manage.py createsuperuser`_
11. Run server
    ```sh
    python manage.py runserver
    ```
12. Login to admin panel - (`http://127.0.0.1:8000/admin/`)
13. Add categories, products, add variations, register user, login, place orders and all features.


## Support
💙 If you like this project, give it a ⭐ and share it with friends!

##
Made with ❤️ and Python
