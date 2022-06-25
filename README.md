aws-mfa-login
--------------
1. Need to install the "jq" library to extract variables from JSON object:
    apt-get install jq
2. Open ~/.bash_profile. Add your environment variable like below. Don't forget to update the text below with your own credentials.
    export $AWS_USER_SERIAL_NUMBER=arn:aws:iam::111111111111:mfa/user.name
2. Need to make your file executable:
    chmod +x aws-login
3. Everytime you want to update the credentials, please use this command below:
    source aws-login
4. Viola!
