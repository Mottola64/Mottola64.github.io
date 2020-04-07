---
layout: post
title:      "My Ruby On Rails Project"
date:       2020-04-07 22:00:16 +0000
permalink:  my_ruby_on_rails_project
---


For my Ruby on Rails project I built *ClientManager*, an application for account managers to use to track their accounts and the deliverables they need to work on for their accounts.

I enjoyed learning Ruby On Rails after Sinatra because it seemed like all the harder parts of Sinatra, specifically the routing and the controller actions were simplified for you.

My Rails project follows the MVC design pattern. The Model View Controller (MVC) design pattern provides a separation of concerns where each part of the application has its own purpose and interacts with the other parts of the application.

The Model is where the data is saved and manipulated, it is the logic portion of an application. Models are typically Ruby classes, and can connect to databases to save data. Views is the front-end portion of an application and are the only part of a web application that a user would interact with. Views are created using .erb files and consist of HTML and embedded Ruby. Controllers are the go-between for models and views. Controllers relay data from the browser to the application and back. Controllers consist of routes that take requests from the browser, run code using the models, and render an .erb file for the users to see.

In my project there were three models: user, account, & deliverable. Users have many accounts and have many deliverables through accounts. One tricky thing that I learned was that I needed to add code in my account model to tell Rails that if an account was deleted, delete all the deliverables that were attached to that account.

```
class Account < ApplicationRecord
    belongs_to :user
    has_many :deliverables, dependent: :destroy
    validates :name, :tier, :industry, :acv, :strategist, presence: true
    accepts_nested_attributes_for :deliverables
 end
```

For this project, I implemented user authentication with Omniauth. After creating the functionality to login with Facebook, I really felt like I was finally creating something relevant in the coding world!
