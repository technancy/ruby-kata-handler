#!/usr/bin/env ruby
# -*- ruby -*-

require 'rake/clean'
require 'rake/testtask'

task :default => :spec

task :spec do
  sh 'rspec --color */*_spec.rb'
end
