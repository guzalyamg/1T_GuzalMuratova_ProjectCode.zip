# 1T_GuzalMuratova_ProjectCode.zip
shop ease bot for final exam


ShopEase Bot – README
1. Project Overview
ShopEase Bot is a shopping bot made in Python using Telegram.
Users can browse categories and products.
Users can select sizes and add products to their cart.
Users can confirm orders.
Admin receives order details automatically.
This project is the final version based on our midterm presentation.

2. Project Requirements
You need:
Python 3.10+
PyCharm (or another Python IDE)
Telegram account
Telegram bot token (create a bot via BotFather)
Required Python libraries:
aiogram
sqlite3 (built-in with Python)
All libraries are listed in requirements.txt.

3. Project Files
Your project folder should include:
bot.py → main bot code
loader.py → bot, dispatcher, and database initialization
database/database.py → all database functions
handlers/catalog.py → buttons and keyboards
images/ → product images folder
config.py → configuration (DB path, token, admin ID)
requirements.txt → all libraries
README.md → this file

4. Setup Instructions
Step 1 – Install Python
Go to python.org and install Python 3.10+
Make sure to check “Add Python to PATH”
Step 2 – Install PyCharm
Download PyCharm Community Edition from jetbrains.com
Install it on your computer
Step 3 – Download Project
Download the ZIP file from submission or your source folder
Extract it to a folder
Step 4 – Open Project in PyCharm
Open PyCharm → Open → select the project folder
Make sure the project interpreter is Python 3.10+
Step 5 – Install Dependencies
Open terminal in PyCharm
Run: pip install -r requirements.txt
5. Configuration
5.1 Bot Token
Open config.py
Replace BOT_TOKEN with your Telegram bot token from BotFather
BOT_TOKEN = "YOUR_TELEGRAM_BOT_TOKEN_HERE"
ADMIN_ID = 1781282864  # replace with your Telegram ID if needed
DB_PATH = "database/shop.db"
5.2 Admin ID
Change ADMIN_ID to your Telegram user ID to receive orders
5.3 Database
Database file: database/shop.db
All tables (categories, products, cart) are created automatically when bot starts
6. How to Run the Bot
Open PyCharm terminal
Make sure your virtual environment is active:
venv\Scripts\activate
Run the bot: python bot.py
The bot will say: Bot is running...
Open Telegram → search your bot → click Start
7. How to Use the Bot
Browsing Products
Click 🛒 Catalog
Choose a category
Choose a product → see its details and image
Selecting Size & Adding to Cart
Click Add to Cart
Choose a size:
Clothes: XS, S, M, L, XL
Shoes/Sneakers: 36, 37, 38, 39, 40
Bot confirms: ✅ Added to cart with size …
Viewing Cart
Click 🛍 My Cart
See products, sizes, and total price
Click ✅ Confirm Order to place order
Cancel Action
Type /cancel → bot cancels current action
Help
Type /help → bot shows commands
8. Admin Actions
Admin receives a message in Telegram with all order details:
Product name
Size
Price
Total
9. Testing the Bot
Test all functions:
Add products to cart
Select size
Confirm order
Cancel action
Help command
10. Notes
All images must be in images/ folder
Database is SQLite → no extra setup required
The project works on a fresh computer if Python and libraries are installed
11. STUDENT
Group Name: COSC 2110 1T
Student Name: Guzal Muratova
