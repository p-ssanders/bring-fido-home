#   bring-fido-home

A static HTML/HTMX/CSS site for the Bring Fido Home dog onboarding business.

##  Running Locally

    python3 -m http.server 9000

##  Contact Form

The contact form uses HTMX to make a POST request to an AWS API Gateway.

The API Gateway acts as a proxy to an AWS Lambda function that parses the form, and sends the contents via e-mail to the proprietor, and persists the JSON in an S3 bucket.