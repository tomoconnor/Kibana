load 'deploy'
load 'config/deploy' # remove this line to skip loading any of the default tasks

default_run_options[:pty] = true

ssh_options[:forward_agent] = true
set :git_enable_submodules, 1
set :deploy_via, :remote_cache
set :use_sudo, false

set :local_user, "deploy"
set :user, "deploy"

set :deploy_to, "/opt/applications/#{application}"

set :copy_strategy, :export
set :deploy_via, :rsync_with_remote_cache

set :default_branch, "kibana-ruby"

set :branch, "kibana-ruby"

task :live do
    role :live, "log01", :primary => true
end


namespace :deploy do

    task :migrate do
        puts "    not doing migrate because not a Rails application."
    end

    task :finalize_update do
    end

    task :start do
        puts "    not doing start because not a Rails application."
    end
  
    task :stop do 
        puts "    not doing stop because not a Rails application."
    end

    task :restart do
        puts "    not doing stop because not a Rails application."
    end

    task :postinstall, :except=>{:no_release=>true} do
        puts "    not doing stop because not a Rails application."
    end
end
