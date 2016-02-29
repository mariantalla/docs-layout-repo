namespace :css do
  desc 'Build PUI stylesheets'
  task :build do
    sh './node_modules/.bin/dr-frankenstyle source/stylesheets/'
  end

  desc 'Update PUI stylesheets'
  task :update do
    sh 'npm update pui-css-all'
    Rake::Task['css:build'].invoke
  end
end
