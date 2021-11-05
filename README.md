# MynTee - An E-Commerce Website

# Table of Contents

- [MYNTEE](#myntee)
- [Table of Contents](#table-of-contents)
  - [Installation](#installation)
  - [Usage](#usage)
  - [Inspiration](#inspiration)
  - [What it does](#what-it-does)
  - [How we built it](#how-we-built-it)
  - [Main features](#main-features)
  - [Tech stack](#tech-stack)
  - [Screenshots](#screenshots)
  - [What's next for MYNTEE](#whats-next-for-myntee)
  - [Demo](#demo)

## Installation

Clone the project repository

``` bash
# change directory
$ cd MYNTEE

# Setup Virtual Environment(LINUX)
$ virtualenv venv
$ source venv/bin/activate

# Install requirements
$ pip install -r requirements.txt

# Migrate db File
$ python manage.py makemigrations
$ python manage.py migrate
```

## Usage

```
# Launch server
$ python manage.py runserver

```
## Inspiration

We wanted to build a one stop application connecting all the users to fashion stores ranging from local shop-owners to established enterprises for effective and smooth fashion items, apparel and accessory discovery. A multi-auth system enabling smart communication, reducing distance gap, providing maximum support to the end users would be really useful and help in this noble cause.


## What it does

We have built a fully functional and innovative AI based portal, Myntee, connecting users to fashion stores ranging from local shop-owners to established enterprises. The multi-auth system enables multiple selling units to interact seamlessly in the same portal. Myntee is equipped with with a virtual tryon assistant where users can upload any picture and our tryon will output your predicted look with the specific apparel. We have a recommender suggesting similar apparels or accessories based on your uploaded wardrobe style images. Also equipped with voice based apparel ordering or even general availability based enquiry - our chatbot serves it all. Along with a real-time rating system to make our models evolve continuously. The genetic algorithm ranking all selling units based on distance, prices, availability and ratings - offering personalized selections to our users. Smooth face-based authentication system; tracking positional coordinates for our recommender system to work upon. The main features are namely SmartConnect - A portal connecting selling stores(independent units, acclaimed fashion stores, local shop-owners) to all users; TryOn - Virtual tryon assistant to let users have an idea of personal look; RecMend - Apparel and accessory recommender based on user uploaded wardrobe style pictures; RealSent - Real time sentiment analysis wrapped star rating system; GenRank - Genetic Algorithm ranking the fashion selling units and VoiceChat - Voice based ordering or enquiry chatbot. 

## How we built it 

We aim to simplify the process of delivery and ordering system packed in a single application. Made in Django and powered by superior quality design, to intrigue users. The frontend is mainly made on full bootstrap and night owl CDN, providing state of the art UI. We have tried to keep the UI/UX transitions as much smooth and user friendly as possible. We decided to use Django as the core of our application as it is powered by Python. All the work is done on the very latest Django version and Python 3.7.3 . Python enabled us to use all the machine learning and recommendation technology to it's full potential. The Django model gives us a total boost by letting us easily override the BASE USER model. Thus, we developed a multi user framework, one for the fashion selling units and another for all our users. If multiple sellers are selling the same product, then the customer is redirected to a new page where all the sellers are displayed selling that particular product based on a genetic ranking algorithm. An user can order from multiple sellers in a single order, which is a big boon too. The user section comes with a first in kind chatbot using RASA NLU. It enables the users to add the desired amount of the products available. Once the word "checkout" is received by the chatbot, the shopping list created by the chatbot is then relayed to the cart. The cart in this model is maintained by a session store. It has several properties to add, delete, clear and initialize the Cart Session. This is an intricate way which also keep in the product ID for filtering. The chatbot has also a voice recognition technology which helps disabled users. The speech recognition and speech to text is achieved by IBM Watson's Speech To Text Converter. We have also looked deep into the Security part of the application very well. It is embedded with a face recognition technology using the facelib and OpenCV library. It becomes a very easy application to register as well. This also provides a two layer security for the application, thus enabling to achieve full trust of the customer. The customer section also comes with a virtual tryon assistant where users can upload any picture and our tryon will output your predicted look with the specific apparel via Tensorflow PosNet. We have a recommender suggesting similar apparels or accessories based on your uploaded wardrobe style images Now coming to the fashion store selling units section , it allows facilities to upload items , and add the categories they want to put it under. A simple dashboard for their sales and orders too is created. The application is wrapped end to end by integrating a stripe payment facility. On a successful order, a mail is received by the customer and also the seller with the order details. The seller only gets the details of the  products he owns. So the SMTP feature is really a boost to the users. Moreover once the order is delivered, the seller can check on the delivered symbol, and a delivered message will go to the customer.

## Main features
	1. Full Authentication via face-recognition
	2. Product Items Add
	3. Apparel and Accessories Addition with Qty, price, etc
	4. Users Can View all categories and browse efficiently
	5. Checkout Page
	6. Wishlists Create
	7. Wishlish Delete
	8. Profile Create
	9. Profile Update
	10.Supplier user
	11.Speech to Text Chatbot
	12.Stripe Payment
	13.AI AUTOMATED ADDITION TO CART
	14.FASHION ITEM REVIEWS VIA SENTIMENT ANALYSIS & GENETIC RANKING ALGORITHM
	15.Recommender ranking top fashion facilities
	16.Genetic algorithm ranking the fashion store facilities selling the same product
	17.Genetic algorithm for ranking uses location, reviews, availability and price
	18.Auto cart addition via voice based chatbot
	19.Product quantity and price enquiry via the voice based chatbot
	20.Virtual tryon assistant
	21.Personalized wardrobe style recommender


## Tech stack
 - Django
 - HTML, CSS, JS
 - Bootstrap4
 - Jquery
 - RASA NLU
 - Tensorflow
 - IBM Watson speech to text
 - Python NLTK
 - Machine Learning algorithms

## Screenshots
<img width="994" alt="Screenshot 2021-11-06 at 12 25 18 AM" src="https://user-images.githubusercontent.com/53152779/140563952-deec3bcc-189f-4487-83df-1971d98d56dc.png">
<img width="994" alt="Screenshot 2021-11-06 at 12 26 54 AM" src="https://user-images.githubusercontent.com/53152779/140564282-0a2afb0e-1669-4f03-968e-6f2c361623ad.png">
<img width="994" alt="Screenshot 2021-11-06 at 12 27 19 AM" src="https://user-images.githubusercontent.com/53152779/140564291-3142f452-bfc4-4b93-a502-917b3d25ab0a.png">
<img width="994" alt="Screenshot 2021-11-06 at 12 27 25 AM" src="https://user-images.githubusercontent.com/53152779/140564300-6e84b3a5-8a86-4f4d-a0e5-88c6b89776a6.png">
<img width="994" alt="Screenshot 2021-11-06 at 12 27 59 AM" src="https://user-images.githubusercontent.com/53152779/140564306-2b63e719-f924-42c3-8bd6-233a1796795a.png">
<img width="994" alt="Screenshot 2021-11-06 at 12 28 32 AM" src="https://user-images.githubusercontent.com/53152779/140564366-6e73e358-6ce1-4f47-ad41-1aab0df262af.png">
<img width="994" alt="Screenshot 2021-11-06 at 12 28 54 AM" src="https://user-images.githubusercontent.com/53152779/140564379-7bef4bc0-c451-4f51-b252-84e96192b09e.png">
<img width="994" alt="Screenshot 2021-11-06 at 12 29 01 AM" src="https://user-images.githubusercontent.com/53152779/140564391-4e58857e-a871-404f-b527-9419fee37afd.png">



## What's next for MYNTEE
- Integration of local languages to our product and expand our products to several more local food distributors for better user experience and wider reach out.
- Make our chatbot robust to handle more complex enquiry or product detail enquiry
- Include a voice based assitant to navigate the entire application

## Demo
https://drive.google.com/drive/folders/1sSD47mzRlf712m4BxKz7xcsJ_rgaUBfg?usp=sharing

