This API works for Tamasia Global Sharia Test.

This is a simple REST Web Service which allow:

  * Login
  * Register
  * Order Product

<a name="installation"></a>
### Installation

#### Copy this project

  1. Clone or Download this repository
  2. Unzip the archive if needed
  3. Copy the folder in the htdocs dir
  4. Start a Text Editor (Atom, Sublime, Visual Studio Code, Vim, etc)
  5. Add the project folder to the editor

#### Install the project

  Go to htdocs dir

  * Windows
  C:\xampp\htdocs

#### Create a database

  Import the tamatest.sql file.

  Or run the SQL script

#### Configure the project

  Change the database configuration in .env file.

### Routes

  * `/register` - post method - This method is used for register the user. e.g.: `http://localhost:8000/api/register` with value name, email, and password

  * `/login` - post method - This method gets a user into the database. e.g.: `http://localhost:8000/api/login` with value email and password

  * `/logout` - get method - This method is used for logout the user. e.g.: `http://localhost:8000/api/logout` with value token we get from login before

  * `/user` - get method - This method is used for get user information. e.g.: `http://localhost:8000/api/user` with value token we get from login before

  * `/products` - post method - This method is used for create product for user. e.g.: `http://localhost:8000/api/products` with value name, price, quantity, and token we get from login before

  * `/order/product/{id}` - put method - This method is used for order product but it still can't be done. e.g.: `http://localhost:8000/api/order/product/{id}` with token we get from login before