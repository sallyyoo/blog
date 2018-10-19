Personal blog system, use python, includes blog display, login, blog management, category management etc.

Will be finished before October 30, 2018.

#### Database tables:  
1.Posts:  
2.Categories  
3.Admin:  
 
#### Route map  
**version 1.1**  
+ 2018/10/11:Create database and Admin table, init Admin account  
+ 2018/10/12:Use blueprints, login, create post table, forge data, display posts with pagination, display categorise, show post detail   
+ 2018/10/15:logout, show certain category posts, add and edit post, delete post, add category and delete category, settings, manage post and category, about, use Flask-Migrate
+ 2018/10/17: links list, books list
+ 2018/10/18: books list, books detail, new book, edit book, delete book, manage book,
category book list, new book cate, manage book category, edit book cate, delete book cate
+ 2018/10/19: debug, errors page
+ Testing  
+ Log
+ Deployment

**version 1.2**  
1.Feature: comments  
2.Feature: links  
3.Feature: full text search  
4.Migrate to MySQL 
#### usage
```
$ pipenv install --dev
$ pipenv shell
$ flask forge
$ flask init
$ flask run
```

#### Flask-migrate usage
```
migrate = Migrate(app, db)
```
1.before migrate, initial(one time)
```
$ flask db init
```
2.generate migrations script
```
$ flask db migrate -m "add comment"
```
3.update database
```
$ flask db upgrade
```
rollback
```
$ flask db downgrade
```
flask db migrate -m "add books and links"