task :default => :build

task :build do
  sh "jekyll build"
end

task :deploy => :build do
  sh "scp -r ./_site/* cwit2015@do.cwit.ca:/var/www/cwit.ca/2015/."
end
