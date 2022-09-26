
task :environment do
  require_relative './config/environment'
end

desc 'opens the pry console'
  task console: :environment do
    Pry.start
  end

namespace :greeting do

  task :hello do
    puts "hello from Rake!"
  end

  desc 'outputs hola to the terminal'
  task :hola do
    puts "hola desde Rake!"
  end

end

namespace :db do
  desc 'migrate changes to your database'
  task migrate: :environment do
    Student.create_table
  end

  desc 'seed the database with dummy data'
  task seed: :environment do
    require_relative './db/seeds'
  end

  
end
