# Solution A

A single template to create all resources.

git clone https://github.com/michael-jobstreet/adt-sola.git

To create the stack:

adt-sola-db-param.json contains the DB credentials. Sent me an email to receive the file or the ParameteValue for:

ParameterKey=ADBUsername
ParameterKey=ADBPassword

Execute in aws-shell
cloudformation create-stack --stack-name "Amaysim-Test-Solution01" --template-body file://adt-sola.json --parameters file://adt-sola-db-param.json

OR

cloudformation create-stack --stack-name "Amaysim-Test-Solution01" --template-body file://adt-sola.json --parameters ParameterKey=ADBUsername,ParameterValue=<?> ParameterKey=ADBPassword,ParameterValue=<?>


To delete the stack:

cloudformatoin delete-stack --stack-name "Amaysim-Test-Solution01"
