## # get-statsector

1. Install the Google Cloud CLI and select right project id cloud-composer-243010
https://cloud.google.com/sdk/docs/install-sdk

2. Set up Application Default Credentials
https://cloud.google.com/docs/authentication/provide-credentials-adc#local-dev

``gcloud auth application-default login``

3. Install requirements

``pip install -r requirements.txt``

4. Test the application

We test the application with a Uvicorn, an ASGI web server implementation for Python.

``pip install uvicorn``

``uvicorn main:app --reload``

**With coordinates **

How to find your coordinates?
On your computer, open Google Maps. Right-click the place or area on the map. This will open a pop-up window. You can find your latitude and longitude in decimal format at the top.

http://127.0.0.1:8000/get-statsector/?lat=50.870&lon=4.705

**With an address string**

http://127.0.0.1:8000/get-statsector/?address=Naamsestraat%202%20215%20Leuven