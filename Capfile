load 'deploy' if respond_to?(:namespace) # cap2 differentiator

set :application, "Terry-Tai-Blog"
set :scm, :git
set :repository, "git@github.com:poshboytl/Terry-Tai-Blog.git"
set :domain, "terrytai.com"
set :use_sudo, false
set :user, "blog"
set :deploy_to, "/home/blog/#{application}"

role :app, domain
role :web, domain

# set :deploy_via, :remote_cache


namespace :deploy do
  task :restart, :roles => :app do
	run "rm #{current_path}/README"
	run "cd #{current_path} && jekyll"
  end

  task :start, :roles => :app do
    # do nothing
  end

  task :stop, :roles => :app do
    # do nothing
  end
  
  task :finalize_update do
    # do nothing
  end
end


