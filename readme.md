# PCW Data Snippet 
This snippet provides access to data from the PCW Unifi Controller for analysis purposes.

# Setup
* Get an access key, secret key, and the bucket name from a PCW staff member 
* Initialize a virtual environment w/ your preferred method - this example will use `pipenv`
`python -m pipenv install`
* Activate the virtual environment 
`python -m pipenv shell`
* Create a `.env` file with the following key/value pairs:
    * BUCKLET_ACCESS_KEY 
    * BUCKET_SECRET_KEY
    * BUCKET_NAME 
    * ENDPOINT_URL

# Use 
`python snippet.py` or `python -m pipenv run python snippet.py`

# Notes 
* This example downloads all 'list_devices' files from the month of October - to adjust the range/endpoints scraped, edit the code in `generate_prefixes`. 
* All files are downloaded into the current working directory!!! To adjust, create a parent director and edit `fname_no_prefix` to include the name - e.g, create folder `pcw` and add `pcw/...`.  