# RubyBlog
https://medium.com/@deallen7/ruby-on-rails-app-build-blog-3d9975a999ae

##### This is a Blog System written by Ruby On Rails

author: Ling Li

ruby version: ruby 2.5.5p157 (2019-03-15 revision 67260) [x86_64-linux-gnu]
rails version: Rails 5.2.3

##### create a new project

$ rails new RubyBlog

##### start project

$ rails s

##### generate a migration for the articles

$ rails g migration create_articles

##### push the migration into a table

$ rake db:migrate


##### update the migration 
$ rake db:rollback

##### test out the connection to the table

$ rails c

$ Article.all

##### add a new article 

article = Article.new(title: "This is my second article", description: "This is my second description")

article.save

##### find article by id

article = Article.find(1)

##### update article record

article.title = "This is an edited second article"

article.save

##### delete article record

article.destroy

##### generate all sorts of paths to update, delete, create, show, etc

rake routes





