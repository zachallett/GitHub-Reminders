require 'rubygems/package_task'
require 'rubygems/specification'
require 'date'
require 'bundler'
require 'qless/tasks'

# task :default => [:spec]

# require 'rspec/core/rake_task'
# desc "Run specs"
# RSpec::Core::RakeTask.new do |t|
#   t.pattern = 'spec/**/*_spec.rb'
# end


namespace :qless do
  task :setup do
    require_relative 'qless_sampler' # to ensure all job classes are loaded

    # Set options via environment variables
    # The only required option is QUEUES; the
    # rest have reasonable defaults.
    ENV['REDISCLOUD_URL'] ||= 'redis://localhost:6379'
    ENV['QUEUES'] ||= 'testing'
  end
end