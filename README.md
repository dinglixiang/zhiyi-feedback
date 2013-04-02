# Feedback
A rails engine for feedback.You can use this in anywhere you want to have a feedback infomation.  

---
### Features

*Using slim to draw the template

*High performance

*.etc

----
### Installation

To install,simply add the following to your Gemfile:

    gem 'feedback',:git => 'git@github.com:YinChangXin/zhiyi-feedback.git'

And then execute:

    $> bundle

After updating your bundle, run the installer:

    $> rails g feedback:install

---
### Usage
    

Add the following code snippet in your project where need to feedback.

    = link_to '','/feedback/feedback_infos/new',:id => "add_feedback", :remote => true, "data-type" => "script",:class =>"btn"

And then,you should touch a new file 'application.slim' ,such as  *app/views/layout/application.slim*

Add the following to 'application.slim',

    doctype html
    html
      head
        title feedback
        = stylesheet_link_tag "application", :media => "all"
        = javascript_include_tag :application
      body
        = yield
---
###Copyright
This project uses MIT-LICENSE and develops by *zhiyisoft*.


