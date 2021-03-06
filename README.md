#Project Video
https://youtu.be/x06CjvRycts

#Inspiration
We deal with new people everyday. May it be buying something from a person we met on Craigslist or paying a food truck driver for that taco -- it's always awkward sharing credit cards or paypal/venmo details with strangers. For true privacy, we need to carry cash, sometimes exact change!

In the digital age of mobile devices, this experience could be easier and more secure. That's why we built CapQR!

#What it does
Anytime you need to share money with a stranger, or receive money from a stranger, you can use the CapQR app. Both the parties need to have this trusted app to send or receive money securely without revealing anyone's identity or sharing any details or turning on Bluetooth or NFC. All you need is an Android (or iOS -- coming soon!) device with a camera.

The sender selects how much money they want to pay. This information is sent with their credentials to a secure server that provides a one time use token that is encoded into a QR code. The payee uses the same app to scan this QR code and presents the server with this token and their credentials. The server transfers the money to both accounts securely and shows success messages to both devices.

That's it! CapQR enables Easy, Secure and Fast Money Transfers!

#How we built it
We built an Android App with two modes to Send and Receive money. The apps are designed with Material design theme and use the google ZXing library to generate and scan QR codes. The apps communicate with the server that is built using Google's app engine cloud endpoints. This server authenticates the clients; handles the money transfer initiation and validation while maintaining anonymity. It talks to api.reimaginebanking.com to actually tranfer money between customer accounts.

## How This Helps User During Financial Crisis
1. Enable common people and small businesses to transact easily, securely.
     * When big banks are unstable, people can still engage in commerce.
     * We're enabling P2P transactions by making them more secure and easy. This enables small businesses and people do more business transactions without paying a fee.
2. Enabling transactions in multiple currencies.
     * We enable this transfers while people are traveling to different countries and might not have cash in local currency.
3. Enabling offline transactions.
     * When natural disasters or other events take down bank networks
4. Enabling people to transact without requiring them to share any information or open any connection (bluetooth/NFC).
     * With a 40 X 40 QR code, we can transfer close to 3000 bytes. With a bigger QR code, we can do more at the cost of difficulty in scanning.

#Challenges we ran into
The main challenge was to get the ZXing library to work as we intended it to function. Once that was done, we spent some time with design and getting the app flow right.

#Accomplishments that we're proud of
* Increasing security of the P2P money transfers
* Beautifully designed Material app
* Working transfer between the payer and payee
* Integration with Capital One API

# What we learned
* ZXing library for generating and capturing QR codes
* Appengine Cloud Endpoints for Android
* Swagger and API design/use
* Capital-one API

# What's next for Cap-QR
We want to test the different flows to make the app reliable. Next, we want to use a real banking API and hopefully release it on Google play store. Finally, we will work on prototyping an iOS version and test it out thoroughly with the flow. Finally, There are also colored QR codes which will help transfer more info and we can put them in a sequence like a GIF or video of QR codes
