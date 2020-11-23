# gitlab-ci.yml
image: node:latest  cache:   paths:   - node_modules/  job:   script:   - apt-get update -qy   - apt-get install -y ruby ruby-dev rubygems-integration   - npm install   - gem install --no-rdoc --no-ri dpl   - dpl --provider=heroku --app=Js-bot467 --api-key=95db4877-7b03-4be3-b3cb-09ffb005af96 
