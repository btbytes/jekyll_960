#!/usr/bin/env ruby
#
#require 'rake'

namespace :gs960 do
  desc "Update 960.gs CSS framework by downloading the latest version" 
  task :update do
    sh "rm -rf css/960gs/*"
    sh "git clone http://github.com/nathansmith/960-Grid-System.git"
    sh "cp -R 960-Grid-System/code/css/*.css css/960gs/"
    sh "rm -rf 960-Grid-System"
  end
end

