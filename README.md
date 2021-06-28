# aws-generate-virtual-mfa-token
AWS Generates New MFA Token

1) Help menu

       $ ./generate-mfa-cli-token.sh

As user trying to run cli commands in aws you will need to generate a new mfa token. Default token life is 12hrs. Once token is generated it will setup a new profile in your ~/.aws/credentials file under profile [mfa]. Make sure you dont already have that profile otherwise it will get overwritten. There are two options that get passed to the script, one is the user name you are currently using to get access through CLI, and second is the virtual token generated by your phone authenticator. 

    $ ./generate-mfa-cli-token.sh <user> <token>
