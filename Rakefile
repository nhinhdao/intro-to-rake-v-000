namespace :greeting do
    desc 'outputs hello to the terminal'
    task :hello do
      puts "hello from Rake!"
    end

    desc 'outputs hola to the terminal'
    task :hola do
        puts "Hola mundo"
    end
end

namespace :db do
    desc 'migrate changes to your database'
    task :migrate => :environment do
        Student.create_table
    end

    desc 'create environment for migrate to work with'
    task :environment do
        require_relative './config/environment'
    end

    desc 'seed the database with some dummy data'
    task :seed do
        require_relative './db/seeds.rb'
    end
end
