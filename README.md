# StockPrice_SMS_Alert 📈

A small project to receive SMS alerts with information about a specific company, using [Twilio](https://shorturl.at/QYo2T), [News API](https://newsapi.org/), and [Alpha Vantage](https://www.alphavantage.co/) APIs.

---

## 📘 How Does It Work?

1. **Stock Data Retrieval**  
   The program takes a company's ticker symbol (e.g., `TSLA` for Tesla) to fetch its stock market information from [Alpha Vantage](https://www.alphavantage.co/).

2. **Price Difference Calculation**  
   - It calculates the difference between the closing price of the current day and the previous day.  
   - Adjustments may apply depending on factors like time zones or non-working days.  

3. **News Retrieval**  
   - If the price difference exceeds 5%, the program fetches the latest news about the company from [News API](https://newsapi.org/).  
   - It selects the first three relevant articles.

4. **SMS Notification**  
   - Using [Twilio](https://shorturl.at/QYo2T), the program sends three SMS messages to the specified phone number with the price difference and news headlines.

If everything works correctly, the receiver will get **three SMS messages** with stock market updates and news for the selected company.

---

## 🚀 Getting Started

### Requirements
- Accounts and credentials for:
  - [Twilio](https://shorturl.at/QYo2T)
  - [News API](https://newsapi.org/)
  - [Alpha Vantage](https://www.alphavantage.co/)
- Basic coding knowledge to modify specific sections of the code.

### Setup Instructions
1. **Obtain API Credentials**  
   Log in to each API platform to generate the necessary credentials like:
   - API key
   - Account SID
   - Token  

2. **Modify the Code**  
   Update the following sections in the code:  

   - **Ticker Symbol**  
     Specify the ticker symbol for the company you want to track (e.g., `TSLA` for Tesla).  
     ![Image 1](https://github.com/user-attachments/assets/5f13267d-95e2-41d7-9283-2cbb32c73ef1)

   - **Alpha Vantage API Key**  
     Insert your Alpha Vantage API key.  
     ![Image 2](https://github.com/user-attachments/assets/afd08b7a-c403-488d-8280-77c071bb1264)

   - **News API Key**  
     Insert your News API key.  
     ![Image 3](https://github.com/user-attachments/assets/2f94406e-d638-4d8f-a175-741c30d6f2bb)

   - **Twilio Credentials**  
     Insert your Twilio account SID and auth token.  
     ![Image 4](https://github.com/user-attachments/assets/00a0d312-55c0-4bd2-9e81-1f96590045e0)

   - **Phone Numbers**  
     Replace the placeholder numbers:
     - `fromNumber`: Your Twilio phone number.  
     - `toNumber`: The recipient's phone number.
     - Note: You must include the `+` prefix.  
     ![Image 5](https://github.com/user-attachments/assets/cdef6b84-2183-47a8-ba2f-c92532305e84)

---

## 📚 Useful Resources

- [Twilio Documentation](https://www.twilio.com/docs/messaging)  
- [News API Documentation](https://newsapi.org/docs)  
- [Alpha Vantage Documentation](https://www.alphavantage.co/documentation/)

---

## 💡 Notes
- Ensure all APIs are correctly configured to avoid errors.  
- Double-check phone numbers and API keys before running the code.    
