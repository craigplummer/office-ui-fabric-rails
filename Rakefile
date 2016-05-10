require "bundler/gem_tasks"
require "rspec/core/rake_task"

RSpec::Core::RakeTask.new(:spec)

task :default => :spec

namespace :assets do
  desc 'Update Office UI Fabric assets'
  task update: :clean do
    sh 'bower install'
    sh 'cp -r bower_components/office-ui-fabric/dist/js/* vendor/assets/js'
    sh 'cp -r bower_components/office-ui-fabric/dist/sass/* vendor/assets/scss'
    
    puts "Updated to the latest version of Office UI Fabric"
  end

  desc 'Remove old Foundation for Sites assets'
  task :clean do
    sh 'rm -rf vendor'
    sh 'mkdir -p vendor/assets/js/ vendor/assets/scss/'
  end
end
