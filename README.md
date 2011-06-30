##staticRack

staticRack is a simple template for easily building static sites that can be deployed to Heroku. The config.ru file can be used to customize this setup and expose further subdomains.

The `sassycoffee` branch has the files setup for development with Sass and CoffeeScript. 

The `sinatra` branch has a Sinatra-backed implementation. `sassycoffee` will build against `sinatra` in the future.

#To install the compass gem:

gem install compass

(use RVM if you aren't already)

#To install CoffeeScript:

Download and install [node.js](https://github.com/joyent/node) or use Brew:

brew install node

Then, install npm, the node package manager:

curl http://npmjs.org/install.sh | sh

#Finally, install coffeescript:

npm install -g coffee-script



For easier use of Sass and CoffeeScript goodness, you can use the following commands to continually compile all the appropriate files:

cd <path-to-project>/public
coffee -o scripts/ -cw coffee/

cd <path-to-project>/public
compass watch