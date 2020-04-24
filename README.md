Serverless workshop

in /backend-restapi and /frontend
npm i

in /frontend

npm run build

npm run start

serverless login

serverless deploy

npm install --save serverless-finch

serverless client deploy

Development

sls info

// deploy one function
sls deploy function -f formSubmit

// run remotely
sls invoke -f formSubmit --data '{"body":{"name":"jeff","email":"jeff@lebowski"}}'

// run local  
sls invoke local -f formSubmit --data '{"body":{"name":"jeff2","email":"jeff@lebowski2"}}'

//  output log
sls invoke -f formSubmit --data '{"body":{"name":"jeff3","email":"jeff@lebowski3"}}' -l

// Stream log
sls logs -f formSubmit -t

// force to deploy everything
sls deploy --force

// list all deploy service version
sls deploy list

// rollback to targeted version 
sls rollback -t 1476790110568


