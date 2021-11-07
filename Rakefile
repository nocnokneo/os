require 'rubygems' if RUBY_VERSION < '1.9.0'

# HOW TO DEPLOY
# Don't forget to run rake gemspec with each release! ... I think...
# then manually edit os.gemspec remove duplicatee rspecs, circular dependency? HUH?
# # then  gem build os.gemspec
# rake build doesn't work???
# sooo...
# basically these days just adjust this file, and VERSION, push it...gem push os-1.1.2.gem

begin
  require 'jeweler'
  Jeweler::Tasks.new do |gem|
    gem.name = "os"
    gem.summary = %Q{Simple and easy way to know if you're on windows or not (reliably), as well as how many bits the OS is, etc.}
    gem.description = %Q{The OS gem allows for some useful and easy functions, like OS.windows? (=> true or false) OS.bits ( => 32 or 64) etc"}
    gem.email = "rogerpack2005@gmail.com"
    gem.homepage = "http://github.com/rdp/os"
    gem.authors = ["rdp", "David McCullars"]
    gem.license = "MIT"
    # gem is a Gem::Specification... see http://www.rubygems.org/read/chapter/20 for additional settings
    # gem.add_development_dependency "fast_require"
    gem.add_development_dependency "rspec", ">= 2.0"
  end
rescue LoadError => e
  puts "Jeweler (or a dependency) not available. Install it with: gem install jeweler #{e}"
end

require 'rspec/core/rake_task'
RSpec::Core::RakeTask.new(:spec)
task :default => :spec

