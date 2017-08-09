# rubyonrailsgems
List of useful gems in Ruby on Rails app

# General
This includes gems which have general purpose.

* [crontab_syntax_checker](https://github.com/bkr/crontab_syntax_checker): This is a gem to chek crontab entry syntax. It is useful when someone wants to verify whether a crobtab entry is valid.

# Web servers
This includes gems related to webservers which would drive the RoR app.

* [unicorn](https://rubygems.org/gems/unicorn/versions/5.1.0): unicorn is an HTTP server for Rack applications designed to only serve fast clients on low-latency, high-bandwidth connections and take advantage of features in Unix/Unix-like kernels.
* [puma](https://github.com/puma/puma): Puma is a simple, fast, threaded, and highly concurrent HTTP 1.1 server for Ruby/Rack applications. It can be well cooperated with JRuby on Rails app.

## Asynchronous jobs
This includes jobs gem which help run aynchronous tasks in a RoR application.

* [delayed_job](https://github.com/collectiveidea/delayed_job): A process based asynchronous task processing gem which can be ran at background. It will fork the specified number of processes to execute the tasks.
* [delayed_job_worker_pool](https://github.com/salsify/delayed_job_worker_pool): A gem based on delayed_job which extends its capability by allowing running the job workers at foreground and recreate jobs which are dead. Moreover, it can reduce memory usage by preloading the app where various workers can share the same application stack.
* [sidekiq](https://github.com/mperham/sidekiq): A thread based task processing gem which uses thread instead of process to process task. This reduces the memory footprint of tasks. It needs to have Redis installed while usng it.

# Performance
This includes gems which are help developers understand the RoR application performance and how to opitimize the application when there is performance issue.

* [derailed_benchmarks](https://github.com/schneems/derailed_benchmarks): It can be ran to check the memory usage of a static gem and a dynamic running RoR app. It provides many commands which can be used to measure performance at different aspects. Including memory, object, gc, time etc.

This list would be updated frequently and pull requests are welcomed.
