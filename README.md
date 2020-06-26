# Monzo Receipt Matcher .NET Core

This combines Monzo with a Google Drive folder that scans for new receipt images files and matches them with the correct transacition.

### How it works:
1. A Receipt Image is added to the folder with the naming style "[MerchantName]-[Amount].png" e.g. "Lidl-5-50.png".

2. A HTTP POST to a function app triggers a message to be send on a service bus queue.

3. Service Bus Reader checks the queue and if the 

![Diagram](App_service_Monzo_Receipt_Matcher.PNG)


## K8s Integration

![Diagram](K8s_Monzo_Receipt_Matcher.PNG)
