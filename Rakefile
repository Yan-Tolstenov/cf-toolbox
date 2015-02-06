begin
  require 'bundler'
  Bundler.require
rescue LoadError
end

task :build do
  sh "middleman build"
end

task :open do
  `open http://0.0.0.0:4567`
end
