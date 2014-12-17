task :default => :build

task :build do
  sh "jekyll build"
end

task :deploy => :build do
  sh "scp -r ./_site/* cwit2015@do.cwit.ca:/var/www/cwit.ca/2015/."
end

task :open do
  sh "open http://www.cwit.ca/2015"
end

task :preview => :build do
  sh "open ./_site/index.html"
end
