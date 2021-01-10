
require "capistrano/setup"
require "capistrano/deploy"

require "capistrano/scm/git"
install_plugin Capistrano::SCM::Git

require 'capistrano/rails/migrations'
require "capistrano/bundler"
require "capistrano/rvm"
require 'capistrano/puma'
install_plugin Capistrano::Puma  # Default puma tasks
# require 'capistrano/rails'
# cap puma:monit:config              # Config Puma monit-service
# cap puma:monit:monitor             # Monitor Puma monit-service
# cap puma:monit:restart             # Restart Puma monit-service
# cap puma:monit:start               # Start Puma monit-service
# cap puma:monit:stop                # Stop Puma monit-service
# cap puma:monit:unmonitor 
  # install_plugin Capistrano::Puma::Workers  # if you want to control the workers (in cluster mode)
  # install_plugin Capistrano::Puma::Jungle # if you need the jungle tasks
  # install_plugin Capistrano::Puma::Monit  # if you need the monit tasks
  # install_plugin Capistrano::Puma::Nginx 

# Load custom tasks from `lib/capistrano/tasks` if you have any defined
Dir.glob("lib/capistrano/tasks/*.rake").each { |r| import r }
