namespace :greeting do
  desc 'outputs hello to the terminal'
    task :hello do
      puts "hello from Rake!"
    end

    desc 'outputs holla to the terminal'
    task :hola do 
      puts "hola de Rake!"
    end 
end 

task :console do 
end 


namespace :db do
  task :environment do
    require_relative './config/environment'
  end
  
  desc 'migrate changes to the data base'
  task :migrate => :environment do 
    Student.create_table 
  end 

  desc 'seed the data with some dummy data'
    task :seed do
      require_relative './db/seeds.rb'
    end 
end 

