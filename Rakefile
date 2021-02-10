

task :environment do
  require_relative './config/environment'
end

namespace :nonsense do
  desc "Print reminder about eating more fruit."
  task :apple do
    puts "Eat more apples!"
  end
end

namespace :greeting do

  desc 'outputs hello to the terminal'
  task :hello do
    puts "hello from Rake!"
  end

  desc 'outputs hello to the terminal'
  task :hola do
    puts 'hola de Rake!'
  end

end 

desc 'creates console'
  task :console do
    puts "console"
  end

namespace :db do
  
  desc 'migrate changes to your database'
  task :migrate => :environment do
    Student.create_table
  end

  desc 'seed the database with some dummy data'
  task :seed do
    require_relative './db/seeds.rb'
  end

end