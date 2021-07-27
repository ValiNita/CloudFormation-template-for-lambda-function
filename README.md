1. Am creat un bucket cu comanda aws s3 mb s3://vn-lambda-function-bucket --region eu-west-1
2. Am ceat documentul yaml ( este in repo )
3. Am creat un stack cu comanda aws cloudformation create-stack --stack-name vn-lambda-stack --template-body file://lambdaf.yml --capabilities CAPABILITY_NAMED_IAM
StackId: arn:aws:cloudformation:eu-west-1:932627707940:stack/vn-lambda-stack/97950e00-eeed-11eb-9194-06871d626f27
4.Am verificat upload/download dar si invocat functia cu comenzile 
aws lambda invoke --invocation-type RequestResponse --function-name HelloLambdaFunction --log-type Tail outputfile.txt;  more outputfile.txt
aws lambda invoke --invocation-type RequestResponse --function-name HelloLambdaFunction --log-type Tail outputfile.txt;  more outputfile.txt
aws lambda invoke --invocation-type RequestResponse --function-name HelloLambdaFunction --log-type Tail outputfile.txt;  more outputfile.txt
output:

ExecutedVersion: $LATEST
LogResult: U1RBUlQgUmVxdWVzdElkOiBhZDMzYmJkYS04MmIyLTQyMDYtYWY0OC1iMGQwYWM5ZWRjMjUgVmVyc2lvbjogJExBVEVTVApFTkQgUmVxdWVzdElkOiBhZDMzYmJkYS04MmIyLTQyMDYtYWY0OC1iMGQwYWM5ZWRjMjUKUkVQT1JUIFJlcXVlc3RJZDogYWQzM2JiZGEtODJiMi00MjA2LWFmNDgtYjBkMGFjOWVkYzI1CUR1cmF0aW9uOiAxLjExIG1zCUJpbGxlZCBEdXJhdGlvbjogMiBtcwlNZW1vcnkgU2l6ZTogMTI4IE1CCU1heCBNZW1vcnkgVXNlZDogNDggTUIJCg==
StatusCode: 200
"HelloEveryone!"

ExecutedVersion: $LATEST
LogResult: U1RBUlQgUmVxdWVzdElkOiBiOTVmOWNkMS01MzVmLTQ3NWUtOTRlMi1hYjlkMzJlNDIzYjAgVmVyc2lvbjogJExBVEVTVApFTkQgUmVxdWVzdElkOiBiOTVmOWNkMS01MzVmLTQ3NWUtOTRlMi1hYjlkMzJlNDIzYjAKUkVQT1JUIFJlcXVlc3RJZDogYjk1ZjljZDEtNTM1Zi00NzVlLTk0ZTItYWI5ZDMyZTQyM2IwCUR1cmF0aW9uOiAxLjM5IG1zCUJpbGxlZCBEdXJhdGlvbjogMiBtcwlNZW1vcnkgU2l6ZTogMTI4IE1CCU1heCBNZW1vcnkgVXNlZDogNDggTUIJCg==
StatusCode: 200
"HelloEveryone!"

ExecutedVersion: $LATEST
LogResult: U1RBUlQgUmVxdWVzdElkOiBlODRhNDNjYy1iZDY2LTQ3NDgtOTI5MS01OThjMTY3NzgyMDQgVmVyc2lvbjogJExBVEVTVApFTkQgUmVxdWVzdElkOiBlODRhNDNjYy1iZDY2LTQ3NDgtOTI5MS01OThjMTY3NzgyMDQKUkVQT1JUIFJlcXVlc3RJZDogZTg0YTQzY2MtYmQ2Ni00NzQ4LTkyOTEtNTk4YzE2Nzc4MjA0CUR1cmF0aW9uOiAxLjQ3IG1zCUJpbGxlZCBEdXJhdGlvbjogMiBtcwlNZW1vcnkgU2l6ZTogMTI4IE1CCU1heCBNZW1vcnkgVXNlZDogNDggTUIJCg==
StatusCode: 200
"HelloEveryone!"



