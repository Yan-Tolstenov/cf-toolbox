begin
  require 'bundler'
  Bundler.require
rescue LoadError
end

desc "Build static site and push to Cloud Foundry"
task :push => [:build, :deploy]

task :build do
  sh "middleman build"
end

task :deploy do
  sh "cf push"
end

task :open do
  `open http://0.0.0.0:4567`
end
