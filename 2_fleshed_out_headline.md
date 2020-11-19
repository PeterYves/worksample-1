## Introduction to rails

 + What is Rails   
 
   Rails is used to deal with Ruby on Rails(RoR). It is a server-side web application framework that uses model–view–controller (MVC) for defining the          communication between databases and user interface of the web application
 + Difference between rails and other programming languages   
 
    Ruby on Rails is an open source framework that runs on ruby progamming language. Ruby an object-oriented language and is faster as the codes runs without     an other execution like converting into machine language. You can access many Rubygems and libraries in your applications
   
## CHAPTER 3. RAILS APPLICATIONS AND EXAMPLES
   
 + Creating new rails application  
   To created a new rails application use the command **rails new appname -d db** For example **rails new WorkSampleApp -d postgresql**  
   this will create application called WorkSampleApp and it will use postgresql database
   **N.B:** using the above command without specifing the database to use, it will use the default and most of the time is sqlite
 + Dealing with postgresql database  
   To access rails postgresql database simply use the command **rails db**. This will take you to the database management terminal where you can view, and update data from the database
 + Rails modeling  
   A Rails Model is a Ruby class that can add database records (think of whole rows in an Excel table), find particular data you're looking for, update        data, or remove data. These common operations are referred to by the acronym CRUD--Create, Remove, Update, Destroy.  
   To generate model in rails use the command `rails generate model ModelName ColumnOneName:ColumnOneType ColumnTwoName:ColumnTwoType`  
   For example `rails generate model User username:string password:string`  this command will create app/models/user.rb and              db/migrate/20130518173035_create_users.rb files. Model can be used for validations and other user data saving acts.  
 + Rails migrations  
 The migration file, which is stored in db/migrate like all other migrations files. Migrations describe the changes we'll be making to our database (though   haven't actually enacted just yet). In this case, the generated migrations file say:  
  class CreateUsers < ActiveRecord::Migration  
  def change  
    create_table :users do |t|  
      t.string :username  
      t.string :password  

      t.timestamps  
    end  
  end  
end  
 + Rails controllers
 + Rails routes
 + Rails views
 + Rails layout
 + Scaffolding
 + Rails application speed issues and solutions 

